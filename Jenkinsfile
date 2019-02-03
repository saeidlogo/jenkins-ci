node{
  stage("SCM Checkout"){
    git "https://github.com/saeidlogo/jenkins-ci"
  }
  stage("Compile-Package"){
    sh "mvn package"
  }
}
