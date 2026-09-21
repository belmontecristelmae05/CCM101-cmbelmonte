# Reflection

## Reflection on the Cloud Data Engineer Activity

Object storage is suitable for storing millions of photos because it is designed to handle large amounts of unstructured data. Photos can be stored as individual objects and can be accessed when needed. This makes object storage useful for applications that allow users to upload many images.

Docker simplified the deployment of MinIO because I did not need to install and configure the storage service manually. I used a Docker command to download and run the MinIO container while also setting the required ports and administrator credentials. This made the deployment process more organized and easier to manage.

A bucket is a storage container used to organize objects in an object storage system. In this activity, I created a bucket named `client-photos` and uploaded an image into it. The image was stored as an object inside the bucket.

Enterprises can protect object storage from physical server failure by using redundant storage, data replication, and distributed systems. These methods help keep data available even when a physical server or storage device fails.

This activity also helped me become more comfortable with the Linux command line. I practiced commands such as `docker pull`, `docker run`, and `docker ps` while deploying and checking the MinIO container. I also learned how to access a service through a port and manage files using an object storage system. Overall, the activity gave me practical experience with Docker, MinIO, and cloud storage concepts.
