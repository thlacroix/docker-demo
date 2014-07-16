Bruild the image with `docker build --tag==s3 .`

Launch the service with `docker run -d -p 4569:4569 --name=s3 s3`

You can also use another container for the data. First create a data container with `docker run -v /mnt/fakes3_root --name=s3-data ubuntu true` and then use this volume from the s3 container by adding `--volumes-from s3-data` when you run the s3 service.
