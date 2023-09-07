# HARINI #
Hello!My self Harini,Iam from Hyderabad.I completed my graduation recently in july 2023.Where i have dream to pursue my masters in abroad.I worked on my dream through out my undergrad and finally right now i am pursuing my masters in NWMSU.

[myimage](image/My_image.jpg)

****

# sports
‘sport’ is defined by its social interpretation as well as its strong association with physical exertion and performance measures.A human activity involving physical exertion and skill as the primary focus of the activity, with elements of competition or social participation where rules and patterns of behaviour governing the activity exist formally through organisations and is generally recognised as a sport.

|Sport Name|Reason|Hours|
|----------|------|-----|
|Cricket|Improves focus|Four|
|Volley Ball|Reduce fat|One|
|Basket Ball|Improves Physical Health|Two|
|Badminton|Improves flexibility|One|

****

# Quotes

>"The more I learn, the more I realize how much I don't know."-*Isaac Newton*

>"Imagination is more important than knowledge." - *Albert Einstein*

# code fencing

Link to Stack overflow:
https://stackoverflow.com/questions/5335273/how-can-i-send-an-email-using-php


PHP Code:
```
<?php
       // from the form
       $name = trim(strip_tags($_POST['name']));
       $email = trim(strip_tags($_POST['email']));
       $message = htmlentities($_POST['message']);

       // set here
       $subject = "Contact form submitted!";
       $to = 'your@email.com';

       $body = <<<HTML
$message
HTML;

       $headers = "From: $email\r\n";
       $headers .= "Content-type: text/html\r\n";

       // send the email
       mail($to, $subject, $body, $headers);

       // redirect afterwords, if needed
       header('Location: thanks.html');
?>
