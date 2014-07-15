Build the image with `docker build --tag=nodeapp .`

You need to run the [MongoDB](../mongodb) database before running this application.

Run this application with `docker run -d -p 3000:3000 --link db:db --name=nodeapp app`

If your S3 service is not on 192.168.59.103:4569, you need to set the `S3_ENDPOINT` and `S3_PORT` like that with the following options: `-e S3_ENDPOINT=192.168.59.103 -e S3_PORT=4569`
