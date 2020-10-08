node('master'){
    stage('demo'){
        echo 'hello world';
    }

    stage('checkout'){
        checkout scm
    }

    stage('build'){
        composer install
    }

    stage('test'){
        sh './vendor/bin/phpunit';
    }
}
