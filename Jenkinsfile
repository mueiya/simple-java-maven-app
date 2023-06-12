node {
    docker.image('maven:3.9.0').inside ('-v /root/.m2:/root/.m2') {
        stages{
            stage("Build") {
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}