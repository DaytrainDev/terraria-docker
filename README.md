# terraria-docker
A Terraria world and Docker config to run it

to start...
docker-compose up

to end....
docker-compose down

to change the loaded world, modify the last line of the Dockerfile (the -world parameter)

run with interactive terminal (useful for creating a new world)
docker run -it -p 7777:7777 -v ./world:/world --name="terraria" ryshe/terraria:latest

run in background (same as running docker-compose up)
docker run -dit -p 7777:7777 -v ./world:/world --name="terraria" ryshe/terraria:latest -world /world/Irgell.wld
