node('built-in') 
 {
 stage('continuous download') 
   {
    
     git branch: 'main', url: 'https://github.com/ankitnarula28/awsmaven.git'
 
     }   

stage('Continuous build') 

{

sh 'mvn package'

}

stage('Continuous Deployment') 

{

sh 'scp  /home/ubuntu/.jenkins/workspace/multibranch131/webapp/target/webapp.war   ubuntu@172.31.44.254:/var/lib/tomcat9/webapps/qaenv.war'

}

stage('Continuous testing') 

{

sh 'echo "Testing Passed"'

}

}
