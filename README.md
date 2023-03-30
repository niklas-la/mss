# Docker Cluster mit PGAdmin

Dieses Git Repository enthält eine Dockerfile, die es Ihnen ermöglicht, einen Docker-Cluster mit Apache NiFi, PostgreSQL und PGAdmin zu erstellen. Mit diesem Cluster können Sie Datenflüsse erstellen und verwalten, sowie eine PostgreSQL-Datenbank und PGAdmin für die Administration nutzen.

## Installation

Um den Docker-Cluster zu erstellen, müssen Sie Docker auf Ihrem Computer installiert haben. Wenn Sie Docker noch nicht installiert haben, können Sie es von der offiziellen Docker-Website herunterladen und installieren.

## Erstellen des Docker-Clusters

Um den Docker-Cluster zu erstellen, öffnen Sie bitte eine Terminal- oder Kommandozeile in dem Verzeichnis, in dem sich die Dockerfile befindet, und führen Sie den folgenden Befehl aus:

`docker-compose up -d`

Dieser Befehl erstellt die Docker-Images und startet die Container für Apache NiFi, PostgreSQL und PGAdmin.

## Zugriff auf PGAdmin

Sie können auf PGAdmin über den Netzwerkalias zugreifen. Standardmäßig ist der Netzwerkalias "pgadmin". Wenn Sie den Container gestartet haben, können Sie auf PGAdmin zugreifen, indem Sie in Ihrem Browser die URL http://localhost:5050 eingeben.

Wenn Sie auf PGAdmin zum ersten Mal zugreifen, müssen Sie sich mit den folgenden Anmeldeinformationen anmelden:

Benutzername: admin@admin.com
Passwort: admin
Zugriff auf Apache NiFi

Sie können auf Apache NiFi über die URL http://localhost:8080/nifi zugreifen. Wenn Sie den Cluster auf einem Remote-Server oder in einer VM ausgeführt haben, müssen Sie stattdessen die IP-Adresse oder den Hostnamen des Servers verwenden, auf dem der Cluster ausgeführt wird.

## Stoppen des Docker-Clusters

Um den Docker-Cluster zu stoppen, können Sie den folgenden Befehl ausführen:

`docker-compose down`

Dieser Befehl stoppt und entfernt die Container und Images des Docker-Clusters. Wenn Sie den Docker-Cluster später wieder starten möchten, können Sie den Befehl docker-compose up -d erneut ausführen.


