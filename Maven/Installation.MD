# Install Maven on AWS EC2 and run a Maven Project in Jenkins

### Prerequisites
1. EC2 RHEL 8.x Instance [Get help here](https://www.youtube.com/watch?v=KDtS6BzJo3A)
   - With Internet Access
   - Security Group with Port `8080` open for internet

## Install Maven
Create a directory /opt/maven
wget https://dlcdn.apache.org/maven/maven-3/3.8.2/binaries/apache-maven-3.8.2-bin.tar.gz [maveninstaller link]
tar -xvzf apache-maven-3.8.2-bin.tar.gz [extract the file]
set path in the .bash_profile as a root
M2_HOME=/opt/maven/apache-maven-3.8.2
M2=$M2_HOME/bin
PATH=$PATH:$M2_HOME:$M2:$HOME/bin

echo $PATH

## Install git
yum install git -y
```

#### **Install maven plugins** 
```
Maven invoker
Maven integration
```

#### Accessing Jenkins

In global tool configuration
Enter MAVEN_HOME path - /opt/maven/apache-maven-3.8.2

Enter the git 
Apply and save 
```
#### Configure Jenkins


### Test Jenkins Jobs



