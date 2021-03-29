pipeline {
    agent any
    
    stages {
        stage ('Compile Stage') {

            steps {
                def mvnhome = tool name: 'MAVEN_HOME', type: 'maven'
                {
                    sh "${mvnhome}/bin/mvn clean compile"
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                 {
                    sh "${mvnhome}/bin/mvn test"
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                  {
                    sh "${mvnhome}/bin/mvn deploy"
                }
            }
        }
    }
}
