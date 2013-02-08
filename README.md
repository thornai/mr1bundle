mr1bundle
- timeline page
- 
- 
- clone here symfony_folder\src\mr1
- 
- composer.json content: 
- 
- {
    "name": "symfony/framework-standard-edition",
    "description": "The \"Symfony Standard Edition\" distribution",
    "autoload": {
        "psr-0": { "": "src/" }
    },
    "require": {
        "php": ">=5.3.3",
        "symfony/symfony": "2.1.*",
        "doctrine/orm": ">=2.2.3,<2.4-dev",
        "doctrine/doctrine-bundle": "1.1.*",
        "twig/extensions": "1.0.*@dev",
        "symfony/assetic-bundle": "2.1.*",
        "symfony/swiftmailer-bundle": "2.1.*",
        "symfony/monolog-bundle": "2.1.*",
        "sensio/distribution-bundle": "2.1.*",
        "sensio/framework-extra-bundle": "2.1.*",
        "sensio/generator-bundle": "2.1.*",
        "jms/security-extra-bundle": "1.2.*",
        "jms/di-extra-bundle": "1.1.*",
        "kriswallsmith/assetic": "1.1.*@dev"
    },
    "scripts": {
        "post-install-cmd": [
            "Sensio\\Bundle\\DistributionBundle\\Composer\\ScriptHandler::buildBootstrap",
            "Sensio\\Bundle\\DistributionBundle\\Composer\\ScriptHandler::clearCache",
            "Sensio\\Bundle\\DistributionBundle\\Composer\\ScriptHandler::installAssets",
            "Sensio\\Bundle\\DistributionBundle\\Composer\\ScriptHandler::installRequirementsFile"
        ],
        "post-update-cmd": [
            "Sensio\\Bundle\\DistributionBundle\\Composer\\ScriptHandler::buildBootstrap",
            "Sensio\\Bundle\\DistributionBundle\\Composer\\ScriptHandler::clearCache",
            "Sensio\\Bundle\\DistributionBundle\\Composer\\ScriptHandler::installAssets",
            "Sensio\\Bundle\\DistributionBundle\\Composer\\ScriptHandler::installRequirementsFile"
        ]
    },
    "extra": {
        "symfony-app-dir": "app",
        "symfony-web-dir": "web"
    }
}

=========
