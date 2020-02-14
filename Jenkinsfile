node {
  stage ('SCM checkout'){
   
  git 'https://github.com/Patilnpriya/hello-world'
  
}
stage ('Complie-Package'){
 def mvnHome = tool name: 'Maven', type: 'maven'
  sh "${mvnHome}/bin/mvn package"
}

}
