pipeline {
    agent any

    stages {
        stage('Delivery') {
            steps {
		    echo 'Deploying package...'
		    echo '== Clean port 8089'
                    echo '== Deploy package'
					bat 'dir'
					bat 'cd ..'
					bat 'dir'
					bat 'mvn -version'
					bat 'mvn clean'
					bat 'mvn install'
					bat 'mvn package'
					bat 'cd target'
					bat 'java -jar target/JenkinsDemo-0.0.1-SNAPSHOT-fat.jar'
            }
        }
    }
}
