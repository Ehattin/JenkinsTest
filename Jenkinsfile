String branchName = env.BRANCH_NAME
String repoUrl = "https://github.com/Ehattin/JenkinsTest.git"

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

        echo 'Here is a message Directly from our Jenkinsfile'
        }

        stage('Run') {

        echo 'Running python script:'


        }


}
