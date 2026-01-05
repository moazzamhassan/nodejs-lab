Create files index.js, package.json and Dockerfile.
Create an EC2 instance in AWS. 
Connect to EC2 instance using the following command:
ssh -i file.pem ubuntu@<IP-Address>
chmod 600 file.pem
curl https://get.docker.com | bash
now goto directory where dockerfile is available and run the following command
docker build -t cicdtest .
docker images
docker run -d --name 3000:3000 cicdtest
docker logs (container-id)
