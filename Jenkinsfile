pipeline {
    agent any
    
        stages {
            stage ('verify git branch') {
                steps {
                    echo "$GIT_BRANCH"
                }
            }
            stage ('shell') {
                steps {
                    sh 'ls'
                }
            }
            stage ('verify git ') {
                steps {
                    echo "the stage is complete"
                }
            }
        }
    }