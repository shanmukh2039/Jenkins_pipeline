pipeline {
    agent any
    
    stages {
        stage ('Compile Stage') {

            steps {
                def mvnhome = tool name: 'MAVEN_HOME', type: 'maven'
                    {
                    sh "${mvnhome}/opt/maven/mvn clean compile"
                    }
                  }
            }
        ) 
	}	 
