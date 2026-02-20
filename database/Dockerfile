# Prefer the official image and a supported version
FROM mysql:8.0
ENV MYSQL_ROOT_PASSWORD=root
ENV MYSQL_USER=root

# Copy initialization SQL (will run only if the data dir is empty)
COPY database.sql /docker-entrypoint-initdb.d/database.sql

EXPOSE 3306

# Optional: set a sane default charset/collation (adjust to your needs)
# You can also drop a my.cnf instead:
# COPY my.cnf /etc/mysql/conf.d/my.cnf 
