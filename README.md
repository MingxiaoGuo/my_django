# my_django
learning django framework
## Install Python3 on Mac
Python2 is pre-installed by default on MacOS, to install Python3:
1. Install brew first.
2. `brew install python3`
## Setup MySQL database in docker
Running a MySQL database in a docker container.
1. Download MySQL image from docker public repo (using version 5.7)
2. Use `docker images` to check if image is successfully downloaded. 
3. Run docker container using downloaded image: `docker run --name my_django_mysql -e MYSQL_ROOT_PASSWORD=root -d mysql/mysql-server:5.7`
4. Use `docker ps -a` to check if container is running.
5. Use `docker exec -it my_django_mysql bash` to log into docker container
6. Connect MySQL using `mysql -u root -proot`
