# Verwende das Node.js Basis-Image
FROM node:16

# Setze das Arbeitsverzeichnis im Container
WORKDIR /app

# Kopiere die package.json und package-lock.json (falls vorhanden)
COPY package*.json ./

# Installiere die Abhängigkeiten
RUN npm install

# Kopiere den Rest des Projekts in das Arbeitsverzeichnis
COPY . .

# Exponiere den Port, auf dem die App läuft (z. B. 5000)
EXPOSE 5000

# Setze den Startbefehl für die Anwendung
CMD ["npm", "start"]

