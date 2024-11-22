# minecraft-bedrock-image

## Run Minecraft: Bedrock Edition Server in a Docker container

Go download the server for Linux from https://www.minecraft.net/en-us/download/server/bedrock and extract the folder into this repo, you will need to rename the extracted folder to `bedrock-server` so it will mount to the Docker container correctly.

Run these commands:
```sh
docker compose up --build -d
docker attach mcserver
```