#!groovy

node {
stage('git')
{
git credentialsId: '9b3da816-6c00-44aa-95f7-9be3905c0c73', url: 'https://github.com/swarup17-debug/Maven-Web-Project-master.git'
}
stage('maven')
{
def mvnHome = tool name: 'My-PC Maven', type: 'maven'
bat "${mvnHome}/bin/mvn clean package"
}
}
