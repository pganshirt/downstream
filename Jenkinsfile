node {
  try {
    stage('checkout') {
      checkout scm
    }
    stage('prepare') {
      sh "git clean -fdx"
    }
    stage('compile') {
      echo "nothing to compile for hello.sh..."
    }
    stage('test') {
      sh "echo hello world"
    }
    stage('package') {
      sh "echo tar -cvzf hello.tar.gz hello.sh"
    }
    stage('publish') {
      echo "uploading package..."
    }
  } finally {
    stage('cleanup') {
      echo "doing some cleanup..."
    }
  }
}
currentBuild.setDescription("923ab4b-SNAPSHOT" + "\n" + "923ab4b-20171117.131148-1-bin" + "\n" + "Branch: master" + "\n" + "Build container: 0.5.4")
