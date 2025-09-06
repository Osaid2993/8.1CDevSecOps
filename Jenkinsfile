pipeline {
  agent any
  stages {
    stage('Stage 1: Build') {
      steps { 
        echo 'Task: compile and package the code. Tool: Maven.' 
      }
    }
    stage('Stage 2: Unit & Integration Tests') {
      steps { 
        echo 'Task: run unit tests, then integration tests. Tools: JUnit via Maven Surefire/Failsafe.' 
      }
    }
    stage('Stage 3: Code Analysis') {
      steps { 
        echo 'Task: static code analysis to check style/bugs. Tool: SpotBugs.' 
      }
    }
    stage('Stage 4: Security Scan') {
      steps { 
        echo 'Task: scan dependencies for CVEs. Tool: OWASP Dependency-Check.' 
      }
    }
    stage('Stage 5: Deploy to Staging') {
      steps { 
        echo 'Task: deploy build to a staging server (e.g., AWS EC2). Tool: Ansible.' 
      }
    }
    stage('Stage 6: Integration Tests on Staging') {
      steps { 
        echo 'Task: run API/E2E tests on staging. Tool: Newman (Postman CLI).' 
      }
    }
    stage('Stage 7: Deploy to Production') {
      steps { 
        echo 'Task: deploy the tested build to production (e.g., AWS EC2). Tool: Ansible.' 
      }
    }
  }
}
