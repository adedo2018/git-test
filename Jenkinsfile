pipeline {
    agent any
    stages {
        stage('One') {
                steps {
                        echo 'Hi, this is Fred from magic land'
			
                }
        }
	    stage('Two'){
		    
		steps {
			input('Do you want to proceed?')
        }
	    }
        stage('Three') {
                when {
                        not {
                                branch "master"
                        }
                }
                steps {
			echo "Hello"
                        }
        }
        stage('Four') {
				steps {
					echo 'Running the integration test..'
				} 
        }
    }
}
