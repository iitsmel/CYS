<img src="https://user-images.githubusercontent.com/68285613/123541941-84905c00-d779-11eb-9101-be389dd359fe.png" width="900" height="400"/>
<img src="https://user-images.githubusercontent.com/68285613/123541947-89eda680-d779-11eb-82df-d08a5e9d18cb.png" width="900" height="400"/>
<img src="https://user-images.githubusercontent.com/68285613/123541956-8d812d80-d779-11eb-947e-f689c2ba1d22.png" width="900" height="400"/>
<img src="https://user-images.githubusercontent.com/68285613/123541965-9114b480-d779-11eb-9809-2128987968f9.png" width="900" height="400"/>

This is the source code from DVWA. First part of verification is to check whether the verification code is input by human users. <br>
Second step is to check whether users entered the same password twice.<br>
<br>

However , there are no specific part of code for stopping other attack such as CSRF, thus attackers might be able to initial attack to cause damage. <br>
In this case, it means that if the attackers uses web which is built like this:<br>
<br>

<img src="https://user-images.githubusercontent.com/68285613/123542160-932b4300-d77a-11eb-97c5-d61ce77bec83.png" width="900" height="400"/>

. When users click in this web, the attack script will forget the decryption attack and sent it to the server. Which will eventually alter users' password.