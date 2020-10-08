node('master'){
    stage('demo'){
        echo 'hello world';
    }

    stage('checkout'){
        checkout scm
    }

    stage('build'){
        shell "composer install"
    }

    stage('test'){
        shell './vendor/bin/phpunit';
    }
}
