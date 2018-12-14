pipeline
{
agent any

    stages
    {
        stage('Compile Stage')
        {
         withMaven(maven: 'maven_5_5_2')
         {
            sh 'mvn clean compile'
         }
        }

        stage('Testing Stage')
        {
         withMaven(maven: 'maven_5_5_2')
         {
            sh 'mvn test'
         }
        }

        stage('Deployment Stage')
        {
         withMaven(maven: 'maven_5_5_2')
         {
            sh 'mvn deploy'
         }
        }
    }
}