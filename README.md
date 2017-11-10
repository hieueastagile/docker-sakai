docker-sakai
==========

# Installation
Check out Sakai source code to local: git@github.com:sakaiproject/sakai.git, then install needed packages:
```bash
cd sakai
mvn install
```
And deploy the app to tomcat folder:
```bash
mvn install sakai:deploy -Dmaven.tomcat.home=<absolute url of docker-sakai/tomcat folder>
```
Then build the container
```bash
docker-compose up --build
```

You can visit http://localhost:8080/portal to see the result (root url won't work).
