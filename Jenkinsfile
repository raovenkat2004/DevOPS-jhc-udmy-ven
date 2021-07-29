node{
   stage('SCM Checkout'){
     git 'https://github.com/raovenkat2004/DevOPS-jhc-udmy-ven'
   }
   stage('Compile Package'){
     // Get maven home path
     def mvnHome = tool name: 'maven-3', type: 'maven'
     sh "${mvnHome}/bin/mvn package"
   }
    stage('Email Notification'){
       mail bcc: '', body: '''Hi, Welcome to Jenkins and Alerts.
       Thanks
       Venkat''', cc: '', from: '', replyTo: '', subject: 'Jenkins Job', to: 'raovenkat15@gmail.com'
   }
}
