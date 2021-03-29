pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(MAVEN_HOME : 'MAVEN_HOME') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(MAVEN_HOME : 'MAVEN_HOME') {
                    sh 'mvn test'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                withMaven(MAVEN_HOME : 'MAVEN_HOME') {
                    sh 'mvn deploy'
                }
            }
        }
    }
}
