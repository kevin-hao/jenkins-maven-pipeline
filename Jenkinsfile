#!/usr/bin/env groovy

pipeline {
    agent any

    tools {
        maven 'maven-jenkins-363'
    }

    stages {
        stage('Build') {
            steps {
                sh "printenv"
                sh "mvn clean test package spring-boot:repackage"
            }
        }
    }
}