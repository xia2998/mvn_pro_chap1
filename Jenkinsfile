pipeline{
     agent any

     tools{
       maven 'maven3'
     }
  
     stages{
       stage('Build'){
           steps{
           	sh "mvn clean package"
           	sh "printenv" //将环境变量打印到console中
           }
       } 
     }
}
