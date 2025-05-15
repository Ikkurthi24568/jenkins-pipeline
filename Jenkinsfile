  //tools section to auto install packages or define path of the packages
  //Tool we can add under pipleline >stages>stage>tools
  //pipeline>tools

   pipeline {
    agent any
        tools{
             maven 'MAVEN_PATH' // this name should match the name under tools section in jenkins
             }
        stages  {
            stage('Maven'){
                        
                steps{
                    echo "****Maven version****"
                    sh 'mvn --version'
                }
            }
            stage('SpecificStage'){   //This is getting mvn details from slave server
                agent{
            label 'java-agent-slave'
        }

        tools{
            jdk 'JDK-17'
        }
                steps{
                    echo "******Executing tools under stage area*****"
                    sh "mvn --version"
                }
            }
        }

   }
