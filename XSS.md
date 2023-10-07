# Summary:
Reflected cross-site scripting (or XSS) arises when an application receives data in an HTTP request and includes that data within the immediate response in an unsafe way.

# Description:
Reflected XSS attacks, also known as non-persistent attacks, occur when a malicious script is reflected off of a web application to the victim's browser.

# POC
## Steps To Reproduce:
Go to : http://localhost/php-inventory-management-system/index.php
![Uploading image.png…]()


On the url, enter payload after url: cuzh4"><script>alert('XSS')</script>rvhmf

Payload: http://localhost/php-inventory-management-system/index.php/cuzh4"><script>alert('XSS')</script>rvhmf



# Impact:
The impact of reflected cross-site scripting (XSS) can be significant and pose various risks to both web applications and users
