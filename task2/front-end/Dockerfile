# Utilise l’image officielle de Nginx
FROM nginx:latest

# Copie les fichiers du front-end dans le dossier web d’Nginx
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copie le fichier de configuration Nginx
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
