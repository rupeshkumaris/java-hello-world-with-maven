pipeline{
    agent any
stage('source code'){
//get the code 
git branch: 'sprint1_develop', url: 'https://github.com/rupeshkumaris/java-hello-world-with-maven.git'
}
stage('Build the Code')  
{
sh 'mvn package'
}  
stage ('Archiving the package')
archiveArtifacts artifacts: '**/*.war', followSymlinks: false
}