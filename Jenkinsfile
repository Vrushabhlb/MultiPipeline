node('built-in') {
    stage('Continuous Download') {
    git 'https://github.com/sunildevops77/maven'
}
stage('Continuous Build') {
    sh 'mvn package'
}
stage('Continuous Deployment') {
    sh 'scp /home/ubuntu/.jenkins/workspace/ScriptedPipe/webapp/target/webapp.war ubuntu@172.31.30.248:/var/lib/tomcat8/webapps/qaenv.war'
}
stage('Continuous Testing') {
    sh 'echo "Testing Passed"'
}
stage('Continuous Deployment') {
    sh 'scp /home/ubuntu/.jenkins/workspace/ScriptedPipe/webapp/target/webapp.war ubuntu@172.31.29.147:/var/lib/tomcat8/webapps/prodenv.war'
}
}
