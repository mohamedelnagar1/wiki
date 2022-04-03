## Production Deployment Notes

- Clone Repo
	- `git clone repo_url`
- Modify 'package.json'
	- set "dev: false"
- Build wiki image
`:repo/wiki# docker build -t wiki -f dev/build/Dockerfile .`
- Create Docker Containers
`:repo/wiki# docker-compose dev/container/docker-compose.yml up`
