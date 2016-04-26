# docker-cloud9

- step 1: pull from repository: git clone https://github.com/truongld/docker-cloud9.git && cd docker-cloud9
- step 2: buid docker image: docker build -t="basecloud9"
- step 3: run new container from the image: docker run -it -d -p 3000:3000 --name=mycloud9 basecloud9
- step 4: start cloud9 from your new container: docker exec mycloud9 pm2 start /etc/pm2_cloud9.json


=> Now you can access to Cloud9 IDE at: http://docker-manchine-ip:3000
or extends basecloud9 to build your customize images