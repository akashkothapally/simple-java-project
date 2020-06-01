node{
  stage('SCM checkout'){
    git credentialsId: 'git-user', url: 'https://github.com/akashkothapally/simple-java-project.git'
  }
  stage('compile-package'){
    sh'mvn package'
  }
}
