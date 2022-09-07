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
	     mail bcc: '',
 	     body: "Hello All,\nBelow points are deployed on UAT ${params.DeploymentMode}, please check and share the status to Development Team. \nDeployed Points:${params.Notes}",
  	     from: 'jenkins@ashokleyland.com', subject: 'ServiceMandi QA Released Points', to: 'prasanna.kumar@ashokleyland.com,HTL_Jayaprakash2@ashokleyland.com'
	    }
	    
	}
}
