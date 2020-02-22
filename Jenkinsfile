node {

     stage('SCM Checkout'){
        git 'https://github.com/Prakash-Org/Helloworld-repo'
     }
     
     stage('Compile-package'){
        // Get maven home path
        def mvnHome =tool name: 'maven 3.5.3', type: 'maven'
        bat "${mvnHome}/bin/mvn clean install"
     }
     
     stage('Email-notification'){
        mail bcc: '', body: 'This is been triggered from Jenkins Job', cc: '', from: 'prakashreddyg0923@gmail.com', replyTo: '', subject: 'Jenkins job', to: 'prakashreddyg0923@gmail.com'
     }
     
          
}
