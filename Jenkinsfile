// This shows a simple example of how to archive the build output artifacts.
node {
        stage('Checkout SCM'){
                git branch: 'master', url: 'git@github.com:Hyder2227/Sample_Angular.git'
        }

        stage('Install node modules'){
                sh "npm install"
        }
        stage('Build'){
                sh "npm run build:ssr"
        }
        stage('Deploy'){
                sh "pm2 restart all"
        }
}
