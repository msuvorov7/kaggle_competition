# kaggle_competition
Template for kaggle

### Register postgres db in pgAdmin
- open 127.0.0.1:5050 in browser
- login with creds in docker-compose.yaml (admin@admin.com/root)
- `docker ps` and find `CONTAINER ID` for postgres
- `docker inspect <CONTAINER ID>` and find value for key `IPAddress`
- register Server (Servers -> Register -> Server -> Connection -> fill fields with `IPAddress`/root/root)

### Model Registry in MLflow
- open 127.0.0.1:9001 in browser
- login with creds in docker-compose.yaml (minioadmin/minioadmin)
- create bucket `arts` as in .env file (`AWS_S3_BUCKET`)