pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('buildDocker') {
      steps {
        build 'Build'
      }
    }

    stage('publish') {
      steps {
        archiveArtifacts 'backed'
      }
    }

  }
}