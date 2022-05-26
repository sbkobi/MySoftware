properties(
    [
        pipelineTriggers(
             [
                 pollSCM('* * * * *')
             ]
        ),
//         parameters(
//             [
//                 string(description: 'What is your name?', name: 'name', defaultValue: "Jack")
//             ]
//         )
    ]
)
pipeline {
    agent any
    stages {
        stage('Stage1') {
            steps {
                echo "Running stage 1"
//                 echo "Got name: '${name}'"
            }
        }
    }
}
