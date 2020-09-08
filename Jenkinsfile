pipeline {
	agent any
	tools{ 
            nodejs 'node'
		} 
	stages
	{
		stage('Checking versions')
		{
			steps{
					sh 'node --version'
					sh 'npm --version'
					sh 'newman --version'
			}
		}
		stage('Run Node & Newman') 
		{	
             
            steps {
                
                    sh 'newman run NewmanAndCI.postman_collection.json'
                  
                }
		}
	}
    
}
		
