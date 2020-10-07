node('master'){
    environment {
        PATH = '/bin:/usr/bin'
    }
    stage('demo'){
        echo 'hello world';
    }

    stage('checkout'){
        checkout scm
    }

    stage('build'){
        sh 'composer install';
    }

    stage('test'){
        sh './vendor/bin/phpunit';
    }
}
