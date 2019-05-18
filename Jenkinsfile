node {
 stage('scm check')
 {
 git 'https://github.com/javahometech/my-app.git'
 }
 stage ('build package')
 {
 def  Home = tool name: 'MK_firsttest', type: 'maven'
  sh "${Home}/bin/mvn package"
 }
 stage ('send email')
 {
  mail bcc: '', body: '''Hi,
  This is test.
  ''', cc: '', from: '', replyTo: '', subject: 'Hello', to: 'rmk2727@gmail.com'
 }

}
