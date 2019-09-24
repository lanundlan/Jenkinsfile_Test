pipeline
{
	agent any
	stage('first stage')
	{	
		echo "first hello"
	}
	stage('second stage')
	{	
		echo "second hello"
	}
	stage('third stage')
	{	
		echo "third hello"
	}
}