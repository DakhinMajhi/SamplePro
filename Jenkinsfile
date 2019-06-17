pipeline {				//indicate the job is written in Declarative Pipeline
    agent any				//agent specifies where the pipeline will execute. 
    stages {
        stage ("clone") {		//an arbitrary stage name
            steps {
                build 'SA_Clone'	//this is where we specify which job to invoke.
            }
	}
	stage ("build") {		//an arbitrary stage name
            steps {
                build 'SA_Build'	//this is where we specify which job to invoke.
            }
	}
	stage ("Gtest") {		//an arbitrary stage name
            steps {
                build 'SA_Gtest'	//this is where we specify which job to invoke.
            }
	}
	stage ("CodeCov_Static") {		//an arbitrary stage name
            steps {
                build 'SA_Codecov'	//this is where we specify which job to invoke.
            }
	}
	stage ("EndtoEnd") {		//an arbitrary stage name
            steps {
                build 'SA_EndToEnd'	//this is where we specify which job to invoke.
            }
	}
	stage ("Fortify") {		//an arbitrary stage name
            steps {
                build 'SA_Fortify'	//this is where we specify which job to invoke.
            }
        }
    }
}
