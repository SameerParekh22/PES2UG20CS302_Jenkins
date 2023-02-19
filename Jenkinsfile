pipeline{
agent any
stages{
stage('Clone Repository'){
steps{
git branch:'main', url : 'https://gith.com/SameerParekh22/PES2UG20CS302_Jenkins.git' }
}
stage('Build'){
steps{
sh 'make -C main' }
}
stage('Test'){
steps{
sh 'main/hello_exec' }
}
stage('Deploy'){
steps{
sh 'echo "Running file" && main' }
}
}
post{
failure{
sh 'echo "Pipeline Failed"' }
}
}

