pipeline {
  agent any
  stages {
    stage('BUILD') {
      steps {
        archiveArtifacts(onlyIfSuccessful: true, artifacts: '**/*.jar', caseSensitive: true, defaultExcludes: true)
        git(url: 'https://github.com/247708153/practice.git', branch: 'master', changelog: true, credentialsId: 'a490de50-3616-469b-95dd-54da354262bf')
      }
    }

  }
}