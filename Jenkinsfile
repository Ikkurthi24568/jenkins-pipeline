// // Agent lable
// pipeline
// {
// agent {
//     label 'java-agent-slave'
// }
// stages{
//     stage("Build"){
//         steps{
//             echo "hello"
//         }
//     }
// }
// }


pipeline
{
agent{
    label 'java-agent-slave'
}
        stages{
                 stage('Build')  {
                                steps{
                                       echo "this is the stage for building MVN app"
                                      }
                                 }
                 stage('Scripted stage'){
                        steps{
                              echo "*****Excute scripted stage*******"
                        scrip{
                         def course ="k8s"
                        if(course == "k8s") {
                        println("Thank you enrolling {$course} course")
                                         }
                        else
                        println("Do learn k8s")
                       }
                            sleep 10 //SECONDS
                 }
             }
        }

}
