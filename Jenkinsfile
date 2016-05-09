node {
   stage 'Stage 1'
   echo 'Hello World 1'
   stage 'Stage 2'
   echo 'Hello World 2'
   stage 'Checkout'
   git 'https://github.com/kulinski/jenkins-docker-example.git'
   stage 'Build'
   docker.image('maven:3.3.9-jdk-8').inside {
    sh 'mvn --version'
 }
}
