//declrative

pipeline{

agent{ docker{ image 'maven:3.6.3'} }

stages{

    stage('build'){

        steps {
         
         echo "build"

        }
    }

    stage('test'){

        steps {

         echo "test"

        }
    }

    stage('intergration test'){

        steps {
         
         echo "intergration test"

        }
    }
}

//post stage actions

post{

    always{

        echo "i run always"
    }

    success{

        echo "i run in success"

    }

    failure{

        echo "i run in failure"
    }

}

}
