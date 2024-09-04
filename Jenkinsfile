pipeline {
 agent any
 stages {
 stage('Clone Repository') {
 steps {
 git 'https://github.com/VineethVK7/Wednesday.git'
 }
 }
 stage('Build') {
 steps {
 sh 'echo "Building the project..."'
 sh 'echo "Your HTML project doesn\'t require any build step!"'
 }
 }
 stage('Deploy') {
 steps {
 // Replace with the appropriate deployment command for your environment
 sh 'ibmcloud login --apikey KAXkMMm29x4mt2U6QgOD5R8UQmw19U0Nd1MhonNq8CU-'
 sh 'ibmcloud cos object-put --bucket wednesdaybglr --key 
index.html --file path/to/local/index.html'
 }
 }
 }
