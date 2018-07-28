pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
               (maven : 'maven_3_5_0') {
                    sh 'mvn clean compile'
                }
            }
        

        stage ('Testing Stage') {

            steps {
                (maven : 'maven_3_5_0') {
                    sh 'mvn test'
                }
            }
        }
       
       stage ('Package Stage') {
       
           steps {
               (maven : 'maven_3_5_0') {
                    sh 'mvn package'
                 }
             }
        }

                }
            }
        }
    }
}
