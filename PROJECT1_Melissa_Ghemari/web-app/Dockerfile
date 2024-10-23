# Utiliser une image de base légère de Python
FROM python:3.9-slim

# Créer un répertoire de travail dans le conteneur
WORKDIR /app

# Copier le contenu du répertoire actuel dans le conteneur
COPY . /app

# Installer les dépendances depuis requirements.txt
RUN pip install -r requirements.txt

# Exposer le port 5000 utilisé par l'application Flask
EXPOSE 5000

# Démarrer l'application Flask
CMD ["python", "app.py"]
