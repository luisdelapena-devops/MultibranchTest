pipeline{
            agent any
            
            environment {
             KEY_ID= 'coredata.pem'
             GIT_AUTHOR_NAME= 'Luis Enrique De La Peña Figueroa'
             GIT_AUTHOR_EMAIL= 'luis.delapena@beeva.com'
             GIT_URL= 'git@gitlab.beeva.mx:raze/be-coredata.git'
            }
            
            stages {

                stage('build') {
                    steps {
                    //build('coredata-ci-cd')
                    echo "this is the value of our local branch"
                    echo "we are in path " 
                    echo pwd
                    echo workspace
                    echo "${PATH}"
                    //echo env.KEY_PATH
                        
                    }
                    }

		        stage("setup environment") {
                    steps {      
                        echo "an empty block of steps generates aa failure :P lol"
                        
                    }
                    }

                stage('Test') {
                    steps {
                    echo 'we are into Test Step'
                      }
                    }
            }

            post{
                always{
                    echo "${KEY_PATH}"
                    echo "All stages are finished"
                    //load('/home/lpena/Documents/projects/SOPHIA/be-coredata/JenkinsFiles/JenkinsfileSetup')

                }
                success{
                    echo "It exec when all stages are success"
                    
                }
                failure{
                    echo "Something was wrong in previous step"
                    echo "It will happend when a stage is failure"
                }

            }

}


