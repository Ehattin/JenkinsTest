String branchName = env.BRANCH_NAME
String repoUrl = "https://github.com/Ehattin/JenkinsTest.git"
node {

        stage('Clone') {
            // Clones the repository
            echo 'Cloning files from (branch: "' + branchName + '" )'
            git url: repoUrl
        }

        stage('git command') {
        echo 'Executing a git command (committed changes):'
        commitChangeset = sh(returnStdout: true, script: 'git diff-tree --no-commit-id --name-status -r HEAD').trim()
        

        }

        stage('Message') {

        echo 'Here is a message directly from Jenkins :) '
        }

        stage('Run') {
        echo 'Running a script:'
           script {
               def data = new Date()
               println(data)
               bat 'wmic computersystem get name'
           }
            echo 'Running the PythonTest File'
            bat 'python --version'
            bat 'python JenkinsTest.py'
        }


}
