pipeline {
  agent any 
      stages {
        stage{
          echo 'excuting yarn...'
          nodejs('Node-18.1.0'){
            sh 'yarn install'
          }
        }
      }
  stage("run backend"){
    steps {
         echo 'executing gradle...'
         withGradle(){
            sh './gradle -v'
          }
       }
    }
  }
}
