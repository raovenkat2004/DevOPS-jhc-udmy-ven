node{
   stage('SCM Checkout'){
     git 'https://github.com/raovenkat2004/DevOPS-jhc-udmy-ven'
   }
   stage('Compile Package'){
     // Get maven home path
     def mvnHome = tool name: 'maven-3', type: 'maven'
     sh "${mvnHome}/bin/mvn package"
   }
}
