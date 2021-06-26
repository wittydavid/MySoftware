properties([pipelineTriggers([pollSCM('*/30 * * * *')])])
node {
    stage("first step"){
        git branch: 'main', url: 'https://github.com/wittydavid/MySoftware.git'
        sh "echo 'If you see this message - that means that main branh in MySoftware repo has changed'"
        sh "cat README.md"
    }
}
