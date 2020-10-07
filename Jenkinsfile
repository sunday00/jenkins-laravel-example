node('master'){
    stage('demo'){
        echo 'hello world';
    }

    stage('checkout'){
        checkout scm
    }

    stage('build'){
        withEnv(["PATH+NOHUP=/usr/bin"]) {
            sh "composer install"
        }
    }

    stage('test'){
        sh './vendor/bin/phpunit';
    }
}
