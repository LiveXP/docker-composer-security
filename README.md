# Docker Composer Security Advisories [![Build Status](https://travis-ci.org/LiveXP/docker-composer-security.svg?branch=master)](https://travis-ci.org/LiveXP/docker-composer-security)

Docker image for Composer Security Advisories Checker

## Usage

You can use this docker image directly from [Docker Hub](https://hub.docker.com/r/livexp/composer-security/) with `livexp/composer-security:latest`.
You can use the script `composer-checker` to easily check a `composer.lock` file inside the current directory. You can specify the location of the lock file with the first parameter `composer-security /app/composer.lock`.

## Gitlab CI

```yaml
image: livexp/composer-security:latest

composer-security:
  stage: test
  script:
    - composer-security
```
