pipeline
{
agent any
stages
{
  stage('scm checkout')
  { steps {  git branch: 'master', url: 'https://github.com/study24/maven-project' 
          
   } }

  stage('code build')
  { steps { withMaven(jdk: 'Java home', maven: 'Maven home') 
   { sh 'mvn clean package'} 
  }
  }
  
}
}
  




  
  
