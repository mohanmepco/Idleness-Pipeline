pipeline {
    agent {
        node {
            label 'master'
        }
    }

    stages {

        stage('Instance Idleness check') {
            steps {
                sh 'echo "Started...!" '
            }
        }
        stage('git clone') {
            steps {
                sh 'rm -r *; git clone https://github.com/mohanmepco/Idleness-Pipeline.git'
            }
        }
		stage('PersmissionToExecute'){
            steps {
                sh 'cd /root/.jenkins/workspace/Idleness/Idleness-Pipeline; chmod 755 Spot-Instance'
            }
        }
    }
}
        
        

        
   
