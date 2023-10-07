# Summary:
Stored cross-site scripting (also known as second-order or persistent XSS) arises when an application receives data from an untrusted source and includes that data within its later HTTP responses in an unsafe way.

# Description:
Stored XSS, also known as Type-1 or Persistent XSS attacks, typically rely on unsanitized user input points for scripts permanently stored on the target servers.

# POC
## Steps To Reproduce:
Go to : http://localhost/php-inventory-management-system/index.php
![Uploading image.png…]()


On the url, enter payload after url: cuzh4"><script>alert('XSS')</script>rvhmf

Payload: http://localhost/php-inventory-management-system/index.php/cuzh4"><script>alert('XSS')</script>rvhmf



# Impact:
The impact of reflected cross-site scripting (XSS) can be significant and pose various risks to both web applications and users
