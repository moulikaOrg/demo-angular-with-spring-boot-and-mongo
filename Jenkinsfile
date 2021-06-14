pipeline{
    agent{
    
        label "slave_lbl"
    }
    stages{
        stage('git'){
            steps{
                git changelog: false, poll: false, url: 'https://github.com/moulikaOrg/demo-angular-with-spring-boot-and-mongo.git'
            }
        }
        stage('build'){
            steps{
                sh 'mvn clean spring-boot:run'
            }
        }
    }
    
    
}
© 2021 GitHub, Inc.
