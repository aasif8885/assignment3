#!groovy

//1
stage 'clone_AssignmentProject'
node {
git 'https://github.com/BitwiseInc/assignment3.git'
}

//2
stage 'Clean'
node{
  sh 'chmod +x gradlew'
  sh './gradlew clean --info'
}

stage 'Unit Test'
node{
  sh './gradlew test --info'
}