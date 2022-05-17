pipeline {
    agent any
stages {
    stage("source code") {
//get the code 
        steps {
    git branch: 'sprint1_develop', url: 'https://github.com/rupeshkumaris/java-hello-world-with-maven.git'
    }
}
    stage("Build the Code") {
        steps {
    sh 'mvn package'
    }
}  
stage ("Archiving the package") {
    steps {
archiveArtifacts artifacts: '**/*.war', followSymlinks: false
    }
 }
}
}


