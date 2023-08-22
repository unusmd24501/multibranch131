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


}
