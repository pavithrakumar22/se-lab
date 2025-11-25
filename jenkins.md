//maven java

new item

maven_build  
freestyle project
git

branches to buid */main

build steps

add build steps
invoke top level maven targets
maven home
clean

add build steps
invoke top level maven targets
maven home
install

add post build action
archive artifacts
**/*

build other projects
maven_test

same
none
delete workspace before build starts

add build steps
copy artifacts from other project
stable build only
**/*
add build steps
invoke top level maven targets
maven home
test

add post build actions
archive the artifacts
maven home
build

create pipeline
maven-pipleine
build pipeline view






new item
pipeline

pipeline{
    agent any
    tools{
        maven 'MAVEN_HOME'
    }
    stages{
        stage('git repo & clean '){
            steps{
            //bat "rmdir /s /q samplemavenjavaproject"
            bat "git clone link"
            bat "mvn clean -f samplemavenjavaproject"
            }
        }
         stage('install'){
            steps{
            bat "mvn install -f samplemavenjavaproject"
            }
        }
         stage('test '){
            steps{
            bat "mvn test -f samplemavenjavaproject"
            }
        }
         stage('package '){
            steps{
            bat "mvn package -f samplemavenjavaproject"
            }
        }
    }
}


*****

