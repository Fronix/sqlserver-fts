# Simple image to use for sqlserver full-text-search

Example docker-compose
```yaml
version: "3.2"
services:
  sqlserver:
    container_name: sqlserver-fts
    image: fronix/sqlserver-fts  
    ports:
      - "1433:1433"
    environment:
      SA_PASSWORD: "V3rYC0MleXp4ssw0Rd"
      ACCEPT_EULA: "Y"
    volumes:
      - "./databases:/var/opt/mssql/data"
```
