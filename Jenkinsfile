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
            }
        }
        
	}
	post
	{
	    always
	    {
	     emailext body: 'test', subject: 'pipeline status', to: 'raghavi.n@ashokleyland.com'   
	    }
	    
	}
}
