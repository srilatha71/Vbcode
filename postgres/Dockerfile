FROM postgres
#ENV POSTGRES_USER=myuser
ENV POSTGRES_ROOT_PASSWORD=mypassword
#ENV POSTGRES_PASSWORD=mypassword
#ENV POSTGRES_DB=mydb
COPY script/*.sh /docker-entrypoint-initdb.d 
#RUN psql -U postgres -c "CREATE DATABASE mydb;"
#RUN psql -U postgres -c "GRANT ALL PRIVILEGES ON DATABASE mydatabase TO myuser;"
EXPOSE 5432
CMD ["postgres"]
