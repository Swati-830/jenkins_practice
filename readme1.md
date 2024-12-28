1.  phle ye 
sudo wget -O /usr/share/keyrings/jenkins-keyring.asc \
  https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key
echo "deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc]" \
  https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
  /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt-get update
sudo apt-get install jenkins

2. 
sudo apt update
sudo apt install fontconfig openjdk-17-jre
java -versionY
openjdk version "17.0.8" 2023-07-18
OpenJDK Runtime Environment (build 17.0.8+7-Debian-1deb12u1)
OpenJDK 64-Bit Server VM (build 17.0.8+7-Debian-1deb12u1, mixed mode, sharing)

Add Security group 8080 port

3. 

sudo apt update
sudo apt upgrade -y
sudo apt install openjdk-11-jdk -y
  curl -fsSL https://pkg.jenkins.io/debian-stable/jenkins.io-2023.key | sudo tee \
  /usr/share/keyrings/jenkins-keyring.asc > /dev/null
    echo deb [signed-by=/usr/share/keyrings/jenkins-keyring.asc] \
    https://pkg.jenkins.io/debian-stable binary/ | sudo tee \
    /etc/apt/sources.list.d/jenkins.list > /dev/null
sudo apt update
sudo apt install jenkins -y

export PATH=$PATH:/path/to/java/bin


sudo systemctl enable jenkins
sudo systemctl start jenkins
sudo systemctl status jenkins




4. 
copy the password and open jenkins with ip and 8080 port
and start jenkins

5. 
sudo vi /etc/sudoers
add this
root    ALL=(ALL:ALL) ALL
jenkins ALL=(ALL) NOPASSWD:ALL


ADD
sudo usermod -aG docker $USER
sudo newgrp docker
sudo chmod 777 /var/run/docker.socket

sudo systemctl restart jenkins


6.
and make pipeline

modify IAM role

7.
In jenkins 
manage pipeline add git

'''

