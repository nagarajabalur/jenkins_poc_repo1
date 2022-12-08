pipeline {
    agent any
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
                        try {
                            echo "building the app"
                            sh "./script.sh"
                        } catch (err) {
                            echo 'Error : ' + err.getMessage()
                        }
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
