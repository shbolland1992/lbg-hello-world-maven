pipeline {
        agent any

        tools {
            // Install the Maven version configured as "M3" and add it to the path.
            maven "M3"
        }

        stages {
                            steps {
                    // Get some code from a GitHub repository

                    git branch: 'main', url: 'YOUR GITHUB REPO URL HERE'
                }
            }
            stage('Compile') {
                steps {
                    // Run Maven on a Unix agent.
                    sh "mvn clean compile"
                }
            }
        }