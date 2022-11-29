# Create Cyberpanel and Install Wordpress on Digital Ocean VPS

1. Create Cyberpanel Image 
------------------------------------------
2. Update DNS Record
* A  |  @   |   IP
* A   |  www  |  IP
------------------------------------------
3. Run Console & Update Server
------------------------------------------
4. Login Cyber Panel 
 > IP:8090

* Username - admin
* Password - Get password Below cord run in console

 ```sh 
 cat .litespeed_password
  ```
------------------------------------------ 
 6. Install Wordpress
------------------------------------------ 
 7. Install SSL

>  IP:8090/websites/domainname
 * Select Re-Write Option and add below code
 
 ```sh   
  RewriteCond %{SERVER_PORT} ^80$
RewriteRule .* https://%{SERVER_NAME}%{REQUEST_URI} [R=301,L]
```
https://user-images.githubusercontent.com/114587041/201469532-d5192a21-dab8-40a6-931e-6471ed33ade3.mp4
