# docker-php-composer
php composer with custom UID to avoid permission issue when using Docker Volume


## how to use it
`docker run  -e LOCAL_USER_ID=$$(id -u $(USER)) --rm -v $$(pwd)/src:/app ngtrieuvi92/composer composer -vvv install`
