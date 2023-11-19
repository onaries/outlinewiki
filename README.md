## outlinewiki

실행방법  
`docker-compose up -d`

## docker-compose.yml 파일 수정

MINIO의 환경변수값을 채워서 사용


## 환경변수 설정
아래의 값을 채워서 사용
`docker.env` 파일로 저장

```bash
# Generate a hex-encoded 32-byte random key. You should use `openssl rand -hex 32`
SECRET_KEY=
UTILS_SECRET=

DATABASE_URL=postgres://
DATABASE_URL_TEXT=postgres://
PGSSLMODE=disable

REDIS_URL=redis://outline-redis:6379

URL=https://
PORT=3000

AWS_ACCESS_KEY_ID=minio
AWS_SECRET_ACCESS_KEY=
AWS_REGION=us-east-2
AWS_S3_ACCELERATE_URL=https://
AWS_S3_UPLOAD_BUCKET_URL=https://
AWS_S3_UPLOAD_BUCKET_NAME=outlinedata
AWS_S3_UPLOAD_MAX_SIZE=81920000
AWS_S3_FORCE_PATH_STYLE=false
#AWS_S3_ACL=private

SLACK_CLIENT_ID=
SLACK_CLIENT_SECRET=

AZURE_CLIENT_ID=
AZURE_CLIENT_SECRET=
AZURE_RESOURCE_APP_ID=

OIDC_CLIENT_ID=
OIDC_CLIENT_SECRET=
OIDC_AUTH_URI=https://
OIDC_TOKEN_URI=https:/
OIDC_USERINFO_URI=https://

OIDC_USERNAME_CLAIM=username
OIDC_DISPLAY_NAME=OpenID
OIDC_SCOPES=openid

```
