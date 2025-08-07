# Image créée à partir d'une image Mariadb (changer les ??? par une image trouvée sur Docker Hub)
FROM mariadb:lts-ubi9

# Défintion du mot de passe pour l'utilisateur "root"
ENV MARIADB_ROOT_PASSWORD=ultrasupersecuredpassword

# Copie d'un fichier de configuration custom
# (le fichier doit être nommé my.cnf)
COPY ./my.cnf /etc/mysql/conf.d/my.cnf
# Copie d'un dump SQL pour initialiser la base de données
# (le fichier doit être nommé dump.sql)
COPY ./dump /docker-entrypoint-initdb.d

