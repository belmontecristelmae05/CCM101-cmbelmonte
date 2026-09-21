# MinIO Deployment

## Docker Command Used

MinIO was deployed using Docker with the following command:

    docker run -d -p 9000:9000 -p 9001:9001 \
    --name minio-server \
    -e "MINIO_ROOT_USER=cloudadmin" \
    -e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
    quay.io/minio/minio server /data --console-address ":9001"

## Web Console Port

The MinIO web console was accessed using port `9001`.

## Bucket Created

The bucket created in MinIO was named `client-photos`.

An image was uploaded to the `client-photos` bucket to verify that the object storage service was working correctly.

## Environment Variables

The `-e` flags were used to set environment variables for the MinIO container.

- `MINIO_ROOT_USER=cloudadmin` sets the administrator username used to log in to the MinIO web console.
- `MINIO_ROOT_PASSWORD=CloudNova2026!` sets the administrator password used to log in to the MinIO web console.

These environment variables configure the administrator credentials when the MinIO container starts.
