node{
  stage("SCM Checkout"){
    git "https://github.com/saeidlogo/jenkins-ci"
  }
  state("Compile-Package"){
    sh "mvn package"
  }
}
