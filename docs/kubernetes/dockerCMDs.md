#connect to docker
  docker login --username AWS --password $(aws ecr get-login-password --region us-east-1) <accountNumber>.dkr.ecr.us-east-1.amazonaws.com

#pull Image from image repository
  docker pull <account>.dkr.ecr.us-east-1.amazonaws.com/<image>:<tag>
  
 #remove image from docker
  docker rmi <image>:<tag>
  
