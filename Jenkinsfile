pipeline {
	  agent any
	  stages {
	    stage ('Build docker image') {
		  steps {
			  sh "docker build -t jenkinstraining.azurecr.io/sample-docker-image-63497:$BUIL_NUMBER ."
		  }
	  }
	  stage ('Push docker image to container registry') {
	    environment {
		    DOCKER_CONFIG = credentials('jenkins-training-docker-config-json')
	    }
	    steps {
	      sh "export DOCKER_COFIG = \"\$(dirname \"\$DOCKER_CONFIG\")\"; docker push jenkinstraining.azurecr.io/sample-docker-image-63497:$BUILD_NUMBER"
	    }
    }
  }
}
