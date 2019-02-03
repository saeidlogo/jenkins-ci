node{
  stage("SCM Checkout"){
    git "https://github.com/saeidlogo/jenkins-ci"
  }
  stage("Compile-Package"){
    def mavenHome=tool name: 'Default maven', type: 'maven'
    sh "${mavenHome}/bin/mvn package"
  }
  stage('Email Notification'){
      mail bcc: '', body: '''Hi Welcome to jenkins email alerts
      Thanks
      ''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'saeidlogo@gmail.com'
   }
}
