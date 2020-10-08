node('master'){
    stage('demo'){
        echo 'hello world';
    }

    stage('checkout'){
        checkout scm;
    }

    stage('build'){
        shell "composer install";
        shell "npm run prod";
        shell "fahsfihfsuiavbilsd";
    }

    stage('test'){
        shell './vendor/bin/phpunit';
    }
}
