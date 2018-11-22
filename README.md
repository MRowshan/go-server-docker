# go-server-docker

Automated CI (Continuous Integration) setup using Docker

Install Docker Compose:
```bash
sudo curl -L "https://github.com/docker/compose/releases/download/1.23.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```
Make file executable:
```bash
sudo chmod +x /usr/local/bin/docker-compose
```
docker-compose command to create pipeline, this should be done in the `go-http-server-ci` folder
```bash
docker-compose up -d
```
Jenkins can be accessed through the public IP address of the vm on port 80 (HTTP Port)

Branches can be accessed from
`http://ip-address/go-server-docker/branch-name`

To change and make branches, clone the 'go-http-server' repo into go-server-docker  
Run `git checkout -b branch-name` to create a branch
Edit and push changes to update the container with the new changes
