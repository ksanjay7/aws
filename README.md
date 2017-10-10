# aws

For Jenkins :
sudo bash
mkdir /var/jenkins_home
sudo chmod -R 777 /var/jenkins_home
docker info
docker run -d -p 8080:8080 -p 50000:50000 -v /var/jenkins_home:/var/jenkins_home --name jenkins jenkins

For Tomcat :

docker run -d --rm -p 8888:8080 -v /var/jenkins_home/workspace/<repopath>/target:/usr/local/tomcat/webapps/ --name tomcat1 tomcat:8.0
To view enable ports and its :8888/<appname>
