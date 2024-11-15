pipeline {
    agent any

    environment {
        JAVA_HOME = "C:/Program Files/Java/jdk-17"
    }

    stages {
        stage('Clean Stage') {
            steps {
                dir("Selenium_TestNG_Maven_Rep_1") {
                    // Clean the project
                    bat 'C:/Users/ShriB/apache-maven-3.9.9/bin/mvn clean'
                }
            }
        }

        stage('Compile Stage') {
            steps {
                dir("Selenium_TestNG_Maven_Rep_1") {
                    // Compile the project
                    bat 'C:/Users/ShriB/apache-maven-3.9.9/bin/mvn compile'
                }
            }
        }

        stage('Install Stage') {
            steps {
                dir("Selenium_TestNG_Maven_Rep_1") {
                    // Install the project
                    bat 'C:/Users/ShriB/apache-maven-3.9.9/bin/mvn install'
                }
            }
        }
    }
}