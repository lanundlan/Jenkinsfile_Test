pipeline
{
	agent any
	stages
	{
		stage('first stage')
		{	
			steps
			{
				echo "first hello"
			}
		}
		stage('second stage')
		{	
			steps
			{
				echo "second hello"
			}
		}
		stage('third stage')
		{	
			steps
			{
				bat 'make check || true' 
                junit '**/target/*.xml' 
			}
		}
		stage('Build') 
		{
            steps {
                bat 'make' 
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true 
            }
        }

	}
}