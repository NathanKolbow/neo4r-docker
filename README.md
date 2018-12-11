# Dockerfile for a {neo4r} sandbox

## How to 

```
docker pull ColinFay/neo4r-docker
docker run -e PASSWORD=plop -e NEOPASS=pouet -d -p 8787:8787 neo4r
```

Change the passwords to whatever you want. :

+ `PASSWORD`: password to access the RStudio session 
+ `NEOPASS`: password to Neo4J (default is neo4j)

Go to http://localhost:8787/, enter with user=rstudio & your password. 

The user for Neo4J is `neo4j` and password for the one defined in `-e NEOPASS`. If you didn't specified anything, it's `neo4j`. 

In the `neo4r-examples` folder, you'll find a series of Rmd to experiement with `neo4r`.

