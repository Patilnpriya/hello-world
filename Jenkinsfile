node {
  stage ('SCM checkout'){
   
  git 'https://github.com/Patilnpriya/hello-world'
  
}
stage ('Complie-Package'){
 def mvnHome = tool name: 'Maven', type: 'maven'
  sh "${mvnHome}/bin/mvn package"
}
  stage('Slack Msg'){
    slackSend baseUrl: 'https://hooks.slack.com/services/', channel: 'jenkins-pipeline-demo', color: 'Good', message: 'Welcome to Slack', tokenCredentialId: 'SlackDemo'
  }

}
