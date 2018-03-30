# "jstormes/lamp" Docker Image Admin tools

  This composer package is to help manage cron jobs, logs and configuration
for PHP applications that live inside a jstormes/lamp derived Docker image.

  This tool interacts directly with the filesystem to enable and disable CRON
jobs and interrogate logs.

  This tool provides an HTML interface that will work regardless of an 
JavaScript front end, allowing debugging outside the AJAX request/response 
flow. 

  This tool expects to be be called from a PSR-7 compliant router.

# Testing

  The testing requires that you have Docker installed.

## First you must run composer install:
    
BASH based system (OS X/Linux)

 `docker run -v $(pwd):/var/www jstormes/loopback-world composer install` 
 
Power Shell system (Windows 10/7)
 
 `docker run -v ${PWD}:/var/www jstormes/loopback-world composer install`
 
CMD systems (Windows 10/7)

 `docker run -v %cd%:/var/www jstormes/loopback-world composer install`
 
## Running tests

BASH based system (OS X/Linux)

 `docker run -v $(pwd):/var/www jstormes/loopback-world phpunit` 
 
Power Shell system (Windows 10/7)
 
 `docker run -v ${PWD}:/var/www jstormes/loopback-world phpunit`
 
CMD systems (Windows 10/7)

 `docker run -v %cd%:/var/www jstormes/loopback-world phpunit`
 
 