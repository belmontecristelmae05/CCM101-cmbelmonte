# MinIO Deployment

## Deployment

MinIO was deployed in KillerCoda using Docker. The container exposed ports 9000 and 9001, with port 9001 used for the MinIO web console.

## Docker Command Used

```bash
docker run -d -p 9000:9000 -p 9001:9001 \
--name minio-server \
-e "MINIO_ROOT_USER=cloudadmin" \
-e "MINIO_ROOT_PASSWORD=CloudNova2026!" \
quay.io/minio/minio server /data --console-address ":9001"
