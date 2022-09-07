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
 	     body: "Hi Srini,pl discuss",
  	     subject: 'Seating arrangement', to: 'srinivasan.babu@hindujatech.com,raghavi.n@ashokleyland.com'
	    }
	    
	}
}
