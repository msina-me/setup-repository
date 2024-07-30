# setup-repository

## Usage
### Getting the project:
```
git clone https://github.com/msina-me/setup-repository.git
cd setup-repository
```

### Running:
```
mkdir /opt/nexus-data && chown -R 200 /opt/nexus-data
docker compose up -d
```

### Setup
After running the `docker compose` you should do the following steps:
1. Setup ssl in nginx proxy manager
1. Setup your preferred repositories in nexus
1. Add hosts in nginx proxy manager

---
## To-Do List:

- [ ] Add a bash script to
  - [ ] Install docker and docker-compose
  - [ ] Run Portaner
  - [ ] Run target docker-compose
- [ ] Add docker-compose file to run:
  - [x] Nexus
  - [x] Nginx proxy manager
  - [x] Squid
  - [ ] GitLab
- [ ] Create a default GitLab runner
