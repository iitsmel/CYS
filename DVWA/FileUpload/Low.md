First step is to view the source code.

```
<?php

**if**( **isset**( $_POST[ 'Upload' ] ) ) {     // Where are we going to be writing to?     $target_path  = DVWA_WEB_PAGE_TO_ROOT . "hackable/uploads/";     $target_path .= basename( $_FILES[ 'uploaded' ][ 'name' ] );

// Can we move the file to the upload folder?     **if**( !move_uploaded_file( $_FILES[ 'uploaded' ][ 'tmp_name' ], $target_path ) ) {

// No         **echo** '<pre>Your image was not uploaded.</pre>';     }     **else** {

// Yes!         **echo** "<pre>{$target_path} succesfully uploaded!</pre>";     } }

?>
```

The purpose of this program is checking whether files have been received or not. It doesn’t contain any type of code such as giving uploaded files size limits or files type limits. Which will lead the attackers to be able to upload virus to attack this website.

Burp Suite comes in hands by this time. It is the middle between client and server thus it can revel how the uploading has been done( and modify the requests that has been sent to the server ).

After uploading the file to DVWA, it shows that the file is successfully uploaded. Which verify the  theory of " Due to lack of limits of uploading files to DVWA. Attackers can sent viruses into DVWA server without being stopped.