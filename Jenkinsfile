pipeline {
  agent any
  stages{
    
  stage('Clone'){
    steps{
      git url: 'https://github.com/ManojM1107/Internals.git',
        branch: 'main'
    }
  }
  stage('Run Script'){
    steps{
      py 'chmod +x add.py'
      py './add.py'
    }
  }
}
}
  
