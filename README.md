# simple-java-docker
A simple java app that runs on docker 

# This is not a automated docker file were you can run it with a docker comapose method 
# This is just for practice pupose to make and under how to run docker containers
# In this repo we will only under how to 
# Step 1: How to build a Dockerfile 
# Step 2: How to build an image out of it 
# Step 3: How to build and run a contaniner out of it 



#### #####

# So to build an Image use command as 

docker build -t <image name> .
# In the above command the term docker will activate the docker engine 
# The term build will start making a image from the provided Dockerfile 
# The term -t is called tag the name with which you want to build the image 
# and then the name of image you want to give 
# . represent the context of the file ie from where to pick the dockerfile , the dot represent the pick the docker file from the current file or also you can provide a path 

docker run -d --name <container name> <image name>
# In the above command the term docker will activate the docker engine 
# The command run will develop a container and start running it 
# The command --name is called name the container with which you want to build and if you dont provide the name docker will itself genrate a random one 
# and then the name of image you want to run the container on.

## sample commands
docker build -t java-project .
docker run java-project
# see there just to show that the container is running and executing i havent name the container but if you use and name the container it will run but then you need to enter command 
docker logs <container_name>
# to the exectued code within 
# when we name the container the container will start exectue and stop, to make the coantiner run continously you need to create a yaml and compose file.