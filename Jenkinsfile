node {
  stage 'Checkout Repository'
  git url: 'https://github.com/jenkins-swisit/user-search-service.git', branch: "master}"

  stage 'Installing Dependencies'
  sh "mvn install"
  
  stage 'Testing'
  sh "mvn test"

  stage 'packaging'
  sh "mvn package"

  

}