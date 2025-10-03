pipeline {
agent any


stages {
stage('Checkout') {
steps {
checkout scm
}
}


stage('Setup') {
steps {
sh 'python3 -m venv venv'
sh '. venv/bin/activate && python -m pip install --upgrade pip && pip install -r requirements.txt'
}
}


stage('Test') {
steps {
sh 'mkdir -p reports'
sh """
. venv/bin/activate
pytest --maxfail=1 --disable-warnings -q \
--junitxml=reports/junit.xml \
--html=reports/report.html --self-contained-html \
--cov=src --cov-report=xml:reports/coverage.xml
"""
}
}


stage('Publish') {
steps {
junit 'reports/junit.xml'
archiveArtifacts artifacts: 'reports/**', fingerprint: true
// If you have HTML Publisher plugin installed:
publishHTML (target: [
allowMissing: false,
alwaysLinkToLastBuild: true,
keepAll: true,
reportDir: 'reports',
reportFiles: 'report.html',
reportName: 'PyTest HTML Report'
])
}
}
}


post {
always {
archiveArtifacts artifacts: 'reports/**', allowEmptyArchive: true
}
}
}
