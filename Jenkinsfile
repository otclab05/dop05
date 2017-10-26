pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
<<<<<<< HEAD
        echo "Continuous Integration on branch ${env.BRANCH_NAME}"
        echo 'Build libraries'
        echo 'Test deployment'
        echo 'Run unittests'
      }
    }
    stage('Deploy') {
      when { not { expression { BRANCH_NAME ==~ /^feature.*/ } } }
      steps {
        echo 'Pack Images'
      }
    }
    stage('Regression') {
      when { not { expression { BRANCH_NAME ==~ /^feature.*/ } } }
      parallel {
        stage('Business') {
          steps {
            echo 'Check business functionality'
          }
        }
        stage('Integration') {
          steps {
            echo 'Check interfaces/integrations'
          }
        }
        stage('Performance') {
          steps {
            echo 'Check performance on load'
          }
        }
        stage('Stability') {
          steps {
            echo 'Run chaos monkeys'
          }
        }
      }
    }
    stage('Acceptance') {
      when { not { expression { BRANCH_NAME ==~ /^feature.*/ } } }
      steps {
        input 'Accept for production?'
      }
    }
    stage('Production') {
      when { not { expression { BRANCH_NAME ==~ /^feature.*/ } } }
      steps {
        echo 'Production deployment'
      }
    }
  }
}
=======
        echo 'Build05'
      }
    }
  }
}
>>>>>>> 18f0b3c932fc2103406cb6cf42c8dada4a4923e5
