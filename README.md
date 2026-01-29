# FirstTest (Docker + GitHub)

## Run with Docker
```bash
docker build -t firsttest:1 .
docker run --rm -p 8080:80 firsttest:1

Then:
```powershell
git add README.md
git commit -m "Add README with run instructions"
git push

services:
  web:
    image: nginx:alpine
    ports:
      - "8080:80"
    volumes:
      - ./index.html:/usr/share/nginx/html/index.html:ro

docker compose up -d
docker compose down
git add compose.yaml
git commit -m "Add docker compose for one-command run"
git push
