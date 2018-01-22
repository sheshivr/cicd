pipeline
{
 agent any
 stages
 {
	stage('one')
	{
		steps
		{
		   echo "test"
		   git 'https://github.com/sheshivr/cicd.git'
		}
	}
	stage('two')
	{
		steps
		{
		   echo "bulid"
	         input 'Waiting for approval'
		   sh 'mvn clean package'

		}
	}
 }
}
