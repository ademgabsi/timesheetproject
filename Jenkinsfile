pipeline{ agent any

    tools {
        jdk 'Java17'     // le nom EXACT configuré dans Jenkins
        maven 'Maven3'   // le nom EXACT configuré dans Jenkins
    }

    stages {

        stage('GIT') {
            steps {
                git branch: 'master',
                    url: 'https://github.com/ademgabsi/timesheetproject.git'
            }
        }

        stage('Compile Stage') {
            steps {
                sh 'mvn clean compile'
            }
        }
    }
}
