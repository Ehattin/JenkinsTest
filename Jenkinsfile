String branchName = env.BRANCH_NAME
String repoUrl = "https://github.com/Ehattin/JenkinsTest.git"

pipeline {
    
    node {

        stage('Clone') {
            // Clones the repository from the current branch name
            echo 'Make the output directory'
            sh 'mkdir -p build'

            echo 'Cloning files from (branch: "' + branchName + '" )'
            dir('build') {
                git branch: branchName, url: repoUrl
        }

        stage('git command') {
        echo 'Executing a git command (pull):'


        }

        stage('Message') {

        echo 'Here is a console message'
        }

        stage('Run') {

        echo 'Running python script:'


        }


    }
}
