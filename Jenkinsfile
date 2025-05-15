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
            stage('SpecificStage'){
                agent{
            label 'java-agent-slave'
        }
                steps{
                    echo "******Executing tools under stage area*****"
                    sh "mvn --version"
                }
            }
        }

   }
