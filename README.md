# Multiple docker container using docker-compose demo

## How to get started:
• Run `docker-compose up` or `docker-compose up -d`    
• On the local machine, go to `http://localhost:4001`

### Docker container crash debugging:
Restart policies:
• `"no"` - never attempt to restart the container if it stops or crashes    
• `always` - If this container stops for any reason, always attempt to restart it (usually for web servers)    
• `on-failure` - Only restart if the container stops with an error code (usually for worker process)    
ª `unless-stopped` - Always restart unless the dev forcibly stops it    

### Container Status with docker-compose
You can run `docker-compose ps` to get the statuses of the containers that are meant to exist within the current local directory (as opposed to `docker ps` in any directory)