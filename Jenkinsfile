node('master') {
    
    stage('preparation') {
       
        git 'https://github.com/jglick/simple-maven-project-with-tests.git'
    }
    
    stage('build') {
       withMaven(maven: 'M3') {
           sh 'mvn -Dmaven.test.failure.ignore clean package'
        }
    }
}
