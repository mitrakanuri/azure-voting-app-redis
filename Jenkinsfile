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
                    sh  '''cd azure-vote/
                            docker images -a
                            docker build -t jenkins-pipeline .
                            docker images -a
                            cd ..
                    '''
                }
            }
            stage ('verify git ') {
                steps {
                    echo "the stage is complete"
                }
            }
        }
    }