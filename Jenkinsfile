String branchName = env.BRANCH_NAME
String repoUrl = "https://github.com/Ehattin/JenkinsTest.git"

pipeline {
    
    node {

        stage('Clone') {
            // Clones the repository
            echo 'Cloning files from (branch: "' + branchName + '" )'
            git url: repoUrl
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
