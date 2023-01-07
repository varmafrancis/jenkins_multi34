node('built-in') 
{
    stage('Continuous Download') 
	{
    git 'https://github.com/sunildevops77/maven.git'
	}
    stage('Continuous Build') 
	{
            sh label: '', script: 'mvn package}

 stage('ContDeployment')
        {

    sh 'scp /home/ubuntu/.jenkins/workspace/jenkins_multi_loans/webapp/target
webapp.war ubuntu@172.31.34.126:/var/lib/tomcat8/webapps/qaenv.war'

        }
}
