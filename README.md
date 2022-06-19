# docker-compose-gog-linux

Docker-compose environment for playing GOG games for Linux in Docker containers.

## Requirements

  - GNU/Linux OS
  - docker (with docker-compose)

## Usage

  1. Clone the project with:
```bash
git clone https://github.com/mlinaric-io/docker-compose-gog-linux
```

  2. Make project.sh executable:
```bash
chmod +x docker-compose-gog-linux/project.sh
```

  3. Move exactly one GOG game (with DLCs) for Linux OS (with the file extension
 .sh) in the "docker-compose-gog-linux" folder. Script search for "start.sh" to 
start the game, so here can be only one game (with multiple DLCs) at the moment.
```bash
cp some_game.sh docker-compose-gog-linux/some_game.sh
```

  4. Move to the docker-compose-gog-linux folder and start project.sh script. 
Click on "Yes", "Next","Accept" and "Finish" until the bureaucratic torture 
ends. Accept the default destination for installation:
```bash
cd docker-compose-gog-linux && ./project.sh start
```

Occasionally you might want to clean docker containers with:
```bash
cd docker-compose-gog-linux && ./project.sh clean
```

## License

docker-compose-gog-linux is licensed under [MIT License](LICENSE)

