node('master'){
    environment {
        PATH = '/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin'
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
