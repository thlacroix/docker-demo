Create the data container with `docker run -v /data ubuntu mkdir /data/db`
Launch a MongoDB container with `docker run -d --name=db dockerfile/mongodb --noprealloc --smallfiles`

To expose publicly the port 27017, add `-p 27017:27017`, or `-P` (you need to run `docker port db 2017` to discover the forwarded port)

You can also build the Dockerfile in this folder with `docker build --tag=mongodb .` and use it instead of `dockerfile/mongodb`
