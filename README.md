
# PHP QA tools and configuration files

  

## _phpcs_/_phpcbf_ - Code beautifier

Install phpcs & phpcbf globally

  

```code
composer global require "squizlabs/php_codesniffer=*"
```

Place **phpcs.xml** in root directory(not in project/public/).

Scan file or directory for issues
```code
phpcs file/dir
```
after scan to fix issues run
```code
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
phpmd file/dir html --report-file report.html phpmd.xml
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

Place **psalm.xml** in root directory(not in project/public/).

Scan file or directory for issues
```code
psalm
```

# Other tools

## _php-cs-fixer_ - PHP coding standard fixer

Install php-cs-fixer
```code
composer global require friendsofphp/php-cs-fixer
```

Run it with command
```code
php-cs-fixer fix file/directory
```

## _phpcpd_ - PHP copy/paste detector
Install phpcpd

```code
composer require --dev sebastian/phpcpd
```

Run it with command
```code
phpcpd file/directory
```

## _phpdcd_ - PHP dead code detector

Install phpdcd
```code

composer require --dev 'sebastian/phpdcd=*'

```

Run it with command
```code
phpdcd file/directory
```

## _phan_ - PHP static analysis tool
  Install phan
```code
    composer require phan/phan
```


## _psalter_ - Fix psalm code
Psalter is installed with psalm.

Run

```code
psalter --issues=MissingReturnTyp
```
or
```code
vendor/bin/psalter --issues=MissingReturnTyp
```

## _iniscan_ - Scanner for PHP.ini
Install iniscan
```code
composer require psecio/iniscan
```
Run it with command
```code
iniscan scan --path=/path/to/php.ini
```

## _phpmnd_ - PHP Magic Number Detector
Install phpmnd
```code
composer require --dev povils/phpmnd
```
Run it with command
```code
phpmnd .(or file name)
```

## .editorconfig
EditorConfig helps maintain consistent coding styles for multiple developers working on the same project across various editors and IDEs. The EditorConfig project consists of a file format for defining coding styles and a collection of text editor plugins that enable editors to read the file format and adhere to defined styles. EditorConfig files are easily readable and they work nicely with version control systems.
