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
                        } catch (Exception e) {
                            echo 'Error : ' + e.toString()
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
