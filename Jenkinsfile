pipeline {
    agent any
        stages {
            try {
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
            } catch (Exception e) {
                echo 'Error : ' + e.toString()
            }
        }
}
