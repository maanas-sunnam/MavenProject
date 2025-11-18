node {

    stage('Clone Repository') {
        git url: 'https://github.com/maanas-sunnam/MavenProject.git'
    }

    stage('Clean') {
        bat "mvn clean -f MavenProject/pom.xml"
    }

    stage('Build') {
        bat "mvn install -f MavenProject/pom.xml"
    }

    stage('Test') {
        bat "mvn test -f MavenProject/pom.xml"
    }

    stage('Package') {
        bat "mvn package -f MavenProject/pom.xml"
    }
}
