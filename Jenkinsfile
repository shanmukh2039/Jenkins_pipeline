node {
	stage('SCM Checkout'){
         git 'https://github.com/shanmukh2039/Jenkins_pipeline.git'
	}	
        stage{
        stage('Compile Stage') {
	def mvnHome = tool name: 'MAVEN_HOME', type: 'maven'
		sh "${mvnHome}/opt/maven/mvn package"
		}
	}
	
}
            
      
 
