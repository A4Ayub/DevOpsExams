node {

	try {
	
		stage('Clone'){
			git clone https://github.com/A4Ayub/DevOpsExams.git/
		}

		stage('Build'){
			docker image build --tag a4ayub/DevOpsExams:1.0 .
		}

		stage('Push'){
			docker login --username=a4ayub --email=robert.ayub@gmail.com
			docker push a4ayub/devopsexams:version_one
		}
	
		stage('Deploy'){
			docker run devopsexams		
		}

	} catch(){
		currentBuild.result = 'FAILED'
		throw err
	}

}
