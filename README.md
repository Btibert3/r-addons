# Personal Docker Image

This image is a derivative of [rocker/hadleyverse](https://github.com/rocker-org/hadleyverse) and extends an already great foundation to add packages that I personally use.  

With the ease of Docker containers, it is extremely simple to fire up a powerful machine with all of the R packages I personally use, along with an RStudio Server interface to that machine.

## Packages

These are the packages that I want in my personal setup.

-  RNeo4j: to add the ability to interface with the Neo4j graph database 
-  stattleshipR: an API to get access to a wide range of sports data 


## Usage

Get the image

```
docker pull btibert3/r-addons
```

Fire up the image

```
docker run -d -p 8787:8787 btibert3/r-addons
```

to run the daemonized container, with the necessary Rstudio Server port exposed.

To verify that it is running

```
docker ps
```

If you want to stop the instance, simply grab the idea from the `docker ps` command and `docker stop <instance id here>`

