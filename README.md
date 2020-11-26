1) 	a) D:\projects>git init ArtifactID
    		Initialized empty Git repository in D:/projects/ArtifactID/.git/

 	b) D:\projects>git clone http://gitlab.abc.local/evam/artifactID.git
    		Cloning into 'evamlistener'...
    		warning: You appear to have cloned an empty repository.
    		//created dir artifactID
    		D:\projects>cd ArtifactID

2)	mkdir -p "${ArtifactID}/src/main/java"
	mkdir -p "${ArtifactID}/src/test/java"
  	mkdir -p "${ArtifactID}/src/main/resources"
  	mkdir -p "${ArtifactID}/src/test/resources"
	
3)	maven pom.xml	

4)
	D:\projects\ArtifactID>mvn clean pacakge-DproxySet=true -DproxyHost=prx_host -DproxyPort=8080 -Dhttp.proxyUser=user -Dhttp.proxyPassword=pw -Djavax.net.ssl.trustStore=D:\path\jdk1.8.0_191\jre\lib\security\cacerts

git rm -r --cached .idea

git status

git commit -m "some comments etc"

git push -u origin master
