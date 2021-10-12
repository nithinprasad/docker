## Demo app - developing with Docker
### Tutorial from [Youtube](https://www.youtube.com/watch?v=3c-iBn73dDE&list=PLy7NrYWoggjxtN4YbSMYFFdpaxb-fR4zC&ab_channel=TechWorldwithNana),
This demo app shows a simple user profile app set up using 
- index.html with pure js and css styles
- nodejs backend with express module
- mongodb for data storage

Mongo Client  are docker-based
UI is Node based

#### To build a docker image from the application

    docker build -t my-app:1.0 .       
    
   Step 1: start mongodb and mongo-express

    docker-compose -f docker-compose.yaml up
    
_You can access the mongo-express under localhost:8080 from your browser_
    
Step 2: in mongo-express UI - create a new database "user-account"

Step 3: in mongo-express UI - create a new collection "users" in the database "user-account"
    
The dot "." at the end of the command denotes location of the Dockerfile.
