node
    {
        stage('Compile Stage')
        {

                sh 'mvn clean compile install'

        }

        stage('Testing Stage')
        {

                sh 'mvn surefire:test -Dtest=*.java'

        }

        stage('Deployment Stage')
        {

                sh 'mvn deploy'

        }

        stage('Package Stage')
        {

                sh 'mvn package'

        }

    }
