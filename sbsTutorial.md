composer create-project symfony/website-skeleton hopitalWeb
cd hopitalWeb
symfony server:start

Creation de user
php bin/console make:user

Update user
php bin/console make:entity

Creation d article
php bin/console make:entity

php bin/console make:migration
php bin/console doctrine:migrations:migrate

php bin/console make:controller UserController
php bin/console make:controller ArticleController

{if I cant run angular due to cannot be loaded because running scripts is disabled on this system:
Run Powershell as admin
Get-ExecutionPolicy
(if it returns Restricted)
Set-ExecutionPolicy Unrestricted
(to verify if it changed)
Get-ExecutionPolicy
}

