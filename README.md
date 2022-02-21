# Jenkins-sample-docker-image
</br>

This repos created for create the docker image and push into ACR.<br/>
<b>DockerFile:</b> <br/>
  This file have basic coding install the curl in target system and copy the README file to home dir. </br>
<b>Jenkinsfile:</b> </br>
  Jenkins file have the pipeline code to build and push the docker image into ACR using Jenkins. <br/>
  1. jenkinstraining.azurecr.io - Name of the ACR
  2. sample-docker-image-63497:$BUIL_NUMBER - Docker image name
  3. $BUIL_NUMBER - env variable used for get the dynamic image version
  4. DOCKER_CONFIG - docker config file
 <br>
 <b>Steps: </b>
 <br>
 1. Create the Jenkins pipeline.
 2. Select the environement as "script scm file".
 3. Save the pipeline.
 4. Build pipeline.
 5. Go and check the docker image in ACR.
 6. Go to ACR --> Repository --> Created/pushed docker image will display.
  
