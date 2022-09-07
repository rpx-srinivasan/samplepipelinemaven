pipeline {
    agent any

    stages 
	{
        stage('Build') 
		{
            steps
			{
                echo 'Building Application.....'
            }
        }
    
	
	    stage('Test') 
		{
            steps
			{
                echo 'Testing Application....'
            }
        }
		stage('Deploy') 
		{
            steps
			{
                echo 'Deploying Application....'
		mail bcc: '', body: 'Test', cc: '', from: '', replyTo: '', subject: 'Test', to: 'raghavi.n@ashokleyland.com'
            }
        }
        
	}
	post
	{
	    always
	    {
	     emailext body: 'Body', subject: 'Test', to: 'raghavi.n@ashokleyland.com'   
	    }
	    
	}
}
