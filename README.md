# Bitbucket pipeline for PHP
This container is specifically built to be used inside of a bitbucket pipeline since it doesn't support multiple container orchestration for now, we need to work around that by having one big container with everything installed.  You can read more on [here](https://bitbucket.org/site/master/issues/12901/use-mysql-docker-image-for-unit-tests-in) and watch the issue over [here](https://bitbucket.org/site/master/issues/12757/ability-to-run-multiple-docker-containers)


For a database I am assuming that sqlite3 will be used, just for the sake of simplicity and speed,something like PerconaDB can be used but there are some issues regarding systemd and how it work inside of containers.

# Installed packages
* php7.0
* composer
* phantomjs
* nodejs v6
* git

# How to use
You can find a simple example of how to use this image inside of bitbucket pipelines in `bitbucket-pipelines.yml`