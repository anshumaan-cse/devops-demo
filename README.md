# devops-demo

## Run locally

```bash
npm install
npm start
```

The app runs on port 3000 and returns `Hello DevOps`.

## Docker usage

```bash
docker build -t devops-demo .
docker run -p 3000:3000 devops-demo
```

## CI/CD

- `ci.yml` runs on every push using GitHub Actions on `ubuntu-latest`.
- `docker.yml` runs on every push and builds the Docker image using the included `Dockerfile`.
