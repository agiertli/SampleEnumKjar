pipeline {
agent {
    node {
        label 'maven'
    }
}
    stages {
        stage('Build') { 
            steps {
                configFileProvider([configFile(fileId: 'maven-settings-kjar', variable: 'MAVEN_SETTINGS_XML')]) {

                sh 'mvn -B -s $MAVEN_SETTINGS_XML -DskipTests clean package' 
            }
        }
    }
}
}