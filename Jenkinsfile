node {

	try {
	
		stage('Clone'){
			git clone https://github.com/A4Ayub/DevOpsExams.git/
		}

		stage('Build'){
			docker image build --tag a4ayub/DevOpsExams:1.0 .
		}

		stage('Push'){
			
		}

		stage('Deploy'){
			
		}

	} catch(){
		currentBuild.result = 'FAILED'
		throw err
	}

}
