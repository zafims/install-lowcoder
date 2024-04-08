$ mkdir lowcoder

$ cd lowcoder

$ curl https://raw.githubusercontent.com/lowcoder-org/lowcoder/main/deploy/docker/docker-compose.yaml -o $PWD/docker-compose.yml

$ docker-compose up -d

----- Check the logs by running this command:---- 

$ docker logs -f lowcoder

---- When you see frontend, backend, redis, and mongo entered the RUNNING state, the Lowcoder service has officially started: -----

---> Visit http://public IP:3000 and click Sign up. 
Lowcoder will automatically create a workspace for you, then you can start building your apps and invite members to your workspace.

----> Update to the latest version

$ docker-compose pull

$ docker-compose rm -fsv lowcoder

$ docker-compose up -d

==================== By Docker Hub ==================

$ hub.docker.com/r/rednow/lowercoder/tags

$ docker pull rednow/lowercoder:latest

$ docker run -d --name lowcoder -p 49160:22 -p 8080:8080 -p 1521:1521 rednow/lowercoder:latest



