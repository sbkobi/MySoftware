properties(
    [
        pipelineTriggers(
             [
                 pollSCM('0,30 * * * *')
             ]
        ),
        parameters(
            [
                string(description: 'What is your name?', name: 'name')
            ]
        )
    ]
)
pipeline {
    agent any

    stages {
        stage('Stage1') {
            steps {
                echo "stage 1"
                echo "Got name: '${name}'"
            }
        }
        stage('Stage2') {
            steps {
                script {
                echo 'Stage 2'
                func1()
                bat 'time /t'
            }
        }
    }
}

def func1(){
    return "Hi from func1"
}
