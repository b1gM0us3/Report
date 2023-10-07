# Summary:
Stored cross-site scripting (also known as second-order or persistent XSS) arises when an application receives data from an untrusted source and includes that data within its later HTTP responses in an unsafe way.

# Description:
Stored XSS, also known as Type-1 or Persistent XSS attacks, typically rely on unsanitized user input points for scripts permanently stored on the target servers.

# POC
## Steps To Reproduce:
Go to : http://localhost/pagekit/admin/site/page/edit?id=2
![image](https://github.com/b1gM0us3/Report/blob/main/Screenshot%202023-10-07%20163121.png)

On Menu Title, enter payload and Save: <script>alert('XSS')</script>
![image](https://github.com/b1gM0us3/Report/blob/main/Screenshot%202023-10-07%20163446.png)

Go to: http://localhost/pagekit/admin/site/page
![image](https://github.com/b1gM0us3/Report/blob/main/Screenshot%202023-10-07%20163609.png)

Access /blog.
![image](https://github.com/b1gM0us3/Report/blob/main/Screenshot%202023-10-07%20163517.png)

# Impact:
The impact of store cross-site scripting (XSS) can be significant and pose various risks to both web applications and users
