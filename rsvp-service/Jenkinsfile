Skip to content
Search or jump to…

Pull requests
Issues
Marketplace
Explore
 
@NadineHernandez 
 The password you provided is weak and can be easily guessed. To increase your security, you must update your password. After September 1st, 2019 we will automatically reset your password. Change your password on the settings page.

Read our documentation on safer password practices.

Learn Git and GitHub without any code!
Using the Hello World guide, you’ll start a branch, write comments, and open a pull request.


1
00NadineHernandez/Hello-Jenkins
 Code Issues 0 Pull requests 0 Projects 0 Wiki Security Insights Settings
Hello-Jenkins/rsvp-service/Jenkinsfile
@NadineHernandez NadineHernandez added jenkins file
5294db5 3 hours ago
34 lines (29 sloc)  608 Bytes
  
pipeline {
    agent any

    stages {

        stage('build') {
            steps {
              bat '''
                 cd rsvp-service
                 ./mvnw -DskipTests clean compile
              '''
            }
        }

        stage('test') {
            steps {
              bat '''
                 cd rsvp-service
                     ./mvnw test
              '''
            }
        }

        stage('deliver') {
            steps {
              bat '''
                 cd rsvp-service
                     ./mvnw -DskipTests install
              '''
            }
        }

    }
}
© 2019 GitHub, Inc.
Terms
Privacy
Security
Status
Help
Contact GitHub
Pricing
API
Training
Blog
About
