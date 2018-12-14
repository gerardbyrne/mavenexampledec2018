pipeline
{
    agent any

    stages
    {
        stage('Compile Stage')
        {
        steps{
                sh 'mvn clean compile'
             }
        }

        stage('Testing Stage')
        {
        steps{
                sh 'mvn surefire:test -Dtest=MyAppTests'
'
             }
        }

        stage('Deployment Stage')
        {
         steps{
                sh 'mvn deploy'
             }
        }
    }
}