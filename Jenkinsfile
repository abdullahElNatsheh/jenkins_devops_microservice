//declrative

pipeline{

//agent{ docker{ image 'maven:3.6.3'} }
agent any

environment{

	dockerHome = tool 'mydocker'
    mavenHome = tool  'mymaven'
	PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
}
stages{

    stage('build'){

        steps {

			sh 'mvn --version'
			sh 'docker version'
			echo "PATH 	$PATH"
			echo "bulid number - $env.BUILD_NUMBER"
         
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
