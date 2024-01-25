pipeline { agent any
stages { stage('Checkout') {
steps { 
//checkout scm
echo 'checkout'
} }
stage('Build') { steps {
script {
// Your build commands here
//sh 'mvn clean install' // Example for Maven build
echo 'mvn clean'
} }
}
stage('Test') { steps {
script {
// Your test commands here
//sh 'mvn test' // Example for Maven test
echo 'mvn test'
} }
}
stage('Artifact') { steps {
script {
// Your artifact creation commands here
//sh 'cp target/your-artifact.jar ./artifacts/' // Example for copying a JAR file
echo 'cp target'
}
} }
stage('Dev') { steps {
script {
// Your deployment to dev commands here
//sh 'echo "Deploying to dev environment"' // Example command
echo 'Deploying to dev environment'
} }
} }
post {
success {
echo 'Pipeline successfully executed!'
}
failure {
echo 'Pipeline failed!' }
} }
