# 503-Htaccess


ErrorDocument 503 /index.html

RewriteEngine On
RewriteBase /
RewriteCond %{REQUEST_FILENAME} !-f
RewriteCond %{REQUEST_FILENAME} !-d
RewriteRule .* /index.html [R=503,L]
ErrorDocument 503 /maintenance.html

//Crie então a página maintenance.html e deixe na raiz da instalação.
