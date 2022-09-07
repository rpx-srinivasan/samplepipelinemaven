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
                echoo 'Testing Application....'
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
 	     body: "testing",
  	     subject: 'summary', to: 'srinivasan.babu@hindujatech.com,raghavi.n@ashokleyland.com'
	    }
	    
	}
}
