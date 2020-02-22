node {

     stage('SCM Checkout'){
        git 'https://github.com/Prakash-Org/Helloworld-repo'
     }
     
     stage('Compile-package'){
        bat 'mvn clean install'
     }
}
