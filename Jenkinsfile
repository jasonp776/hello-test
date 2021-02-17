pipeline {
   agent any

   parameters {
      string(name: 'userName', description: 'Name of user to say hello', defaultValue: 'jasonp')
   }

   stages {
      stage('Hello') {
         steps {
            sh """
               echo Hello ${params.userName}!
               """
         }
      }
      stage('Next') {
          steps {
             ls -l
          }
      }
   }
}
