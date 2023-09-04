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

//stage("tomcatdeployment") 
//{
//sh 'cp /home/ec2-user/.jenkins/workspace/myfirstpipeline/target/*.war /home/ec2-user/tomcat/apache-tomcat-9.0.65/webapps'
\\}
\\}
}
}
