## Error 404 for AKAI

Link: http://404.akai.org.pl/


### Nginx configuration
```
error_page   404  /notfound.html;
location = /notfound.html {
        ## your 404.html file parent directory
        root   /usr/share/nginx/html/error_pages/custom404/;
        internal;
}
location /notfound.css {
        alias /usr/share/nginx/html/error_pages/custom404/notfound.css;
}
location /favicon.ico {
        alias /usr/share/nginx/html/error_pages/custom404/favicon.ico;
}
location /logo-akai.png {
        alias /usr/share/nginx/html/error_pages/custom404/logo-akai.png;
}
```
