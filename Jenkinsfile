pipeline {
    agent any
    try {
        stages {
            stage("init") {
                steps {
                    script {
                    echo "initializing the app"
                    }
                }
            }
            stage("build") {
                steps {
                    script {
                        echo "building the app"
                        sh "./script.sh"
                    }
                }
            }
            stage("test") {
                steps {
                    script {
                        echo "testing the app"
                    }
                }
            }
            stage("deploy") {
                steps {
                    script {
                        echo "deploying the app"
                    }
                }
            }
        }
    }
    catch(err) {
        echo "ERROR: ${err}"
    }
}
