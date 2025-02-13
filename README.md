# lab8

1-1.4 ทำตามสเต็ป

2-2.5 ทำตามสเต็ป

2.6
docker container run hello-world
![image](https://github.com/user-attachments/assets/a16b246d-7f34-4d3b-b0d3-f83832263403)


3.2
docker run -p 8100:80 nginx
![image](https://github.com/user-attachments/assets/893710ba-d16c-4f65-8a9c-14f688724469)

3.6 touch index.html ==> create index.html
    vi index.html  => press i and add your name then esc + ctrl : and wq 

    cat to check is there have name that your type

3.9
![image](https://github.com/user-attachments/assets/17238cfb-43a8-4dd2-8bbb-6d0b4bb34046)


docker run --rm --privileged multiarch/qemu-user-static --reset -p yes

docker run -d -p 8080:80 -e NAME="C H A Y O D O M" dto80/environment-docker-example

4.2
![image](https://github.com/user-attachments/assets/093b9a85-7d96-4050-8df9-6d4b93b534cf)

5.4
docker run --name mysql-container --network my-network -e MYSQL_ROOT_PASSWORD=รหัสตัวเอง -d mysql:latest

5.5
docker run --name phpmyadmin-container --network my-network -d -p 8102:80 -e PMA_HOST=mysql-container phpmyadmin/phpmyadmin

5.6 
root
รหัส
![image](https://github.com/user-attachments/assets/189ca052-3176-4ee6-bac0-48edf6aa467d)


5.10

![image](https://github.com/user-attachments/assets/2a2dc6b4-81dc-417f-be65-df493f70a5ab)



6.
  ![image](https://github.com/user-attachments/assets/f35575b2-05a2-49d3-9b0e-5291191131f4)
admin
pass
   ![image](https://github.com/user-attachments/assets/f409856d-bee4-4fef-aeb8-2624e0df9382)

command

docker run -d --name mongodb
-e MONGODB_ROOT_USER=root
-e MONGODB_ROOT_PASSWORD=password123
-p 27017:27017 bitnami/mongodb:latest

docker run -d --name mongo-express --link mongodb:mongo
-p 8081:8081
-e ME_CONFIG_MONGODB_ADMINUSERNAME=root
-e ME_CONFIG_MONGODB_ADMINPASSWORD=password123
-e ME_CONFIG_MONGODB_ENABLE_ADMIN=true
mongo-express:latest

docker rm -f mongo-express

docker run -d --name mongo-express --link mongodb:mongo -p 8081:8081
-e ME_CONFIG_MONGODB_ADMINUSERNAME=root
-e ME_CONFIG_MONGODB_ADMINPASSWORD=password123
-e ME_CONFIG_MONGODB_ENABLE_ADMIN=true
-e ME_CONFIG_MONGODB_SERVER=mongo
mongo-express:latest

