node('nodejs') {
    stage('Checkout') {
        git branch: 'main',
            url: 'https://github.com/zeus-helios/do400-pipelines-control.git'
    }
    stage('Backend Tests') {
        sh 'node ./backend/test.js'
    }
    stage('Frontend Tests') {
        sh 'node ./frontend/test.js'
    }
}
