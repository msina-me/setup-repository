# setup-repository

## Usage
### getting the project:
```
git clone https://github.com/msina-me/setup-repository.git
cd setup-repository
```

### running:
```
mkdir /opt/nexus-data && chown -R 200 /opt/nexus-data
docker compose up -d
```

### setup
After running the `docker compose` you should do the following steps:

1. allow every one to connect to your proxy
  ```
  sed 's|http_access deny all|http_access allow all|g' /opt/squid/squid.conf 
  ```
1. setup ssl in nginx proxy manager
1. setup your preferred repo in nexus


To-Do List:

- [ ] Add a bash script to
  - [ ] Install docker and docker-compose
  - [ ] Run Portaner
  - [ ] Run target docker-compose
- [ ] Add docker-compose file to run:
  - [x] Nexus
  - [x] Nginx proxy manager
  - [x] squid
  - [ ] GitLab
- [ ] Create a default GitLab runner
