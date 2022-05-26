properties(
    [
        pipelineTriggers(
             [
                 pollSCM('* * * * *')
             ]
        ),
        parameters(
            [
                string(description: 'What is your name?', name: 'name', default: "Jack")
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
    }
}
