# terraria-docker
A Terraria world and Docker config to run it

this is a WIP, does not work automatically yet

to run manually, make sure you have docker installed, have port 7777 open, then run the below command from the repo root folder

docker run -it -p 7777:7777 -v ./world:/world --name="terraria" ryshe/terraria:latest
