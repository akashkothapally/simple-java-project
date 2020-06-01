node{
  stage('SCM checkout'){
    git credentialsId: 'git-user', url: 'https://github.com/akashkothapally/simple-java-project.git'
  }
  stage('compile-package'){
    //get maven home path
    def mvnHome = tool name: 'M2_HOME', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
}
