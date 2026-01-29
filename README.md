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
