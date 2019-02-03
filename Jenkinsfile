node{
  stage("SCM Checkout"){
    git "https://github.com/saeidlogo/jenkins-ci"
  }
  stage("Compile-Package"){
    def mavenHome=tool name: 'Default maven', type: 'maven'
    sh "${mavenHome}/bin/mvn package"
  }
}
