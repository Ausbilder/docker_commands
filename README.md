# docker_commands
contains usefull docker commands

# stop all containers
sudo docker stop $(sudo docker ps -a -q)

# remove all stopped containers
sudo docker rm $(sudo docker ps -a -q)

# cleanup volumes 
sudo docker volume rm $(sudo docker volume ls -qf dangling=true)
