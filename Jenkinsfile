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
				sh 'make check || true' 
                junit '**/target/*.xml' 
			}
		}
	}
}