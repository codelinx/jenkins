pipeline {
  agent any
  
  stages {
    stage('build') {
      steps{
        sh 'java -d . src/*.java'
        sh 'echo Main-class: Rectangulator > MANIFEST.MF'
        sh 'jar -cvmf MANIFEST.MF rectangle.jar *.class'
      }
    }

  }
}
