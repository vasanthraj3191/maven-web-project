node {
    stage("Code checkout")
    {
     git credentialsId: 'ae36b7f4-c0b2-4a3a-b08d-7f828d09f5eb', url: 'https://github.com/vasanthraj3191/maven-web-project.git'   
    }
    stage("maven")
    {
        bat "mvn clean package"
    }
    stage("sonar")
    {
        bat "mvn sonar:sonar"
    }
    
}
