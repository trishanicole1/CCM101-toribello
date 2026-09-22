# MinIO Deployment Documentation

## Docker Command Used
docker run -d -p 9000:9000 -p 9001:9001 --name minio-server -e "MINIO_ROOT_USER=cloudadmin" -e "MINIO_ROOT_PASSWORD=CloudNova2026!" pgsty/minio:latest server /data --console-address ":9001"

Note: The official minio/minio Docker image is no longer available since MinIO stopped publishing images in October 2025 and archived their repo in April 2026. The community fork pgsty/minio (SILO) was used instead as a working S3-compatible replacement.

## Access Details
- Web Console Port: 9001
- API Port: 9000
- Bucket Created: client-photos

## Explanation of Environment Variables
- MINIO_ROOT_USER: sets the admin username used to log into the web console.
- MINIO_ROOT_PASSWORD: sets the admin password paired with the root user.

These variables configure secure login credentials at container startup instead of using insecure default credentials.

## Verification Steps
1. Ran docker ps to confirm the container was running.
2. Accessed port 9001 via KillerCoda's Traffic/Ports tab.
3. Logged in with the configured credentials.
4. Created a bucket named client-photos.
5. Uploaded a sample file to confirm the server worked.
