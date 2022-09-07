node('built-in') {
    stage('Continuous Download_master') {
    git 'https://github.com/vrushabh583/hello-word'
}
stage('Continuous Build_master') {
    sh label: ' ', script: 'mvn package'
}
}
