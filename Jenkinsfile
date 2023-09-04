pipeline{
  agent any
   tools {
         maven 'maven'
    }
stages 
  {
stage("codecheckout") {
steps
  {
  git credentialsId: 'github', url: 'git@github.com:DevOps-Traning/Maven-Web-Project.git'
}
}

stage("mavenbuild")
{
steps {
  sh "mvn clean package"
}
}
  }
}

