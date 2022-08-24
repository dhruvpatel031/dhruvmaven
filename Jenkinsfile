pipeline{
  agent any
  stages{
    stage("master branch")
    {
      steps{
        git branch: 'main', url: 'https://github.com/dhruvpatel031/dhruvmaven.git'
      }
    }
    stage("dev branch")
    {
      steps{
        git branch: 'dev-dhruv', url: 'https://github.com/dhruvpatel031/dhruvmaven.git'
      }
  }
    stage("build")
    {
      steps{
      bat "mvn clean install"
      }
    }
}
}
