pipeline {
    agent any


    stages {
        
        
        stage('Deployment') {
            steps {
                sshagent(['deployment-tomcat']) {
                  sh "scp -o StrictHostKeyChecking=no /var/lib/jenkins/workspace/Maven_build_job/webapp/target/webapp.war ec2-user@13.233.186.156:/opt/apache-tomcat-9.0.73/webapps"
}
                
            }
        }
    
    }
}
