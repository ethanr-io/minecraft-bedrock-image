# minecraft-bedrock-image

## Run Minecraft: Bedrock Edition Server in a Docker container

Go download the server for Linux from https://www.minecraft.net/en-us/download/server/bedrock and extract the folder into this repo, you will need to rename the extracted folder to `bedrock-server` so it will mount to the Docker container correctly.

Run these commands to build the docker image, start the container, and attach the session:
```sh
docker compose up --build -d
docker attach mcserver
```

Use `docker stop mcserver` and `docker start mcserver` to stop and start the server, and `docker attach mcserver` to attach to the server CLI
