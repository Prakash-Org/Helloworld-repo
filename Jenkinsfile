node {

     stage('SCM Checkout'){
        git 'https://github.com/Prakash-Org/Helloworld-repo'
     }
     
     stage('Compile-package'){
        // Get maven home path
        def mvnHome =tool name: 'maven 3.5.3', type: 'maven'
        bat "${mvnHome}/bin/mvn clean install"
     }
}
