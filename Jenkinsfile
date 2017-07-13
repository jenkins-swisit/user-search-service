node {
  stage: 'Environment Variables'
  sh "env"

  stage 'Checkout Repository'
  git url: 'https://github.com/jenkins-swisit/user-search-service.git', branch: "${env.BRANCH_NAME}"

  stage 'Installing Dependencies'
  sh "mvn install"
  
  stage 'Testing'
  sh "mvn test"

  stage 'packaging'
  sh "mvn package"

  

}