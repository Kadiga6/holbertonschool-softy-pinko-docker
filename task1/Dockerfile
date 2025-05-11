# Utilise l'image officielle d'Ubuntu
FROM ubuntu:latest

# Met à jour les paquets du système et effectue une mise à jour des paquets installés
RUN apt-get update && apt-get upgrade -y

# Affiche "Hello, World!" lorsque le conteneur est exécuté
CMD echo "Hello, World!"

# Installe python3
RUN apt-get install -y python3 python3-pip

# Supprime la restriction de gestion externe des paquets Python si nécessaire
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED

# Installe flask via pip3
RUN pip3 install flask

# Définit le répertoire de travail
WORKDIR /app

# Copie le fichier api.py dans l'image Docker
COPY api.py /app/api.py

# Commande pour lancer le serveur Flask
CMD ["python3", "api.py"]
