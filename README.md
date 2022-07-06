# PHP QA tools and configuration files 

## _phpcs_/_phpcbf_ - Code beautifier
Install phpcs & phpcbf globally

```code
composer global require "squizlabs/php_codesniffer=*"
```
Place **phpcs.xml** in root directory(not in project/public/).
Scan file or directory for issues
```sh
    phpcs file/dir
```
after scan to fix issues run 
```sh
    phpcs file/dir
```
## _phpmd_ - PHP mess detector

Install phpmd globally
```code
    composer global require phpmd/phpmd
```
Place **phpmd.xml** in root directory(not in project/public/).
Scan with command
```code
    phpmd file/dir html -report-file report.html phpmd.xml
```
Report with errors will be saved in **report.html**
## _phpstan_ - PHP static analysis tool
Install **phpstan** globally

```code
    composer global require phpstan/phpstan
```
Place **phpstan.neon** in root directory(not in project/public/).
Run command 
```code
    phpstan analyse -c phpstan.neon
```
## _psalm_ - PHP static analysis tool
Install **psalm** globally
```code
    composer global require vimeo/psalm
```

# Other tools


## _php-cs-fixer_ - PHP coding standard fixer

## _phpcpd_ - PHP copy/paste detector

## _phpdcd_ - PHP dead code detector

## _phan_ - PHP static analysis tool

## _psalter_ - Fix psalm code 

## _iniscan_ - Scanner for PHP.ini

## _phpmnd_ - PHP Magic Number Detector
