# WordPress Docker Image with WP-CLI

This repository contains the Dockerfile for the autobuild of [wordpress-with-wp-cli](https://hub.docker.com/r/hardeepasrani/docker-wordpress-with-wp-cli/) Docker image.

The Dockerfile uses the official WordPress image and adds [wp-cli](http://wp-cli.org/).

To use, simply run: 

```
docker run --name <containername> hardeepasrani/docker-wordpress-with-wp-cli
```

For all other configuration items, please see the official Docker WordPress [ReadMe](https://github.com/docker-library/docs/tree/master/wordpress).

After you've completed the WordPress installation via the browser, you call the standard wp-cli commands via `docker exec`. For example, to install and activate the Quark theme:

```
docker exec <containername> wp theme install latte
docker exec <containername> wp theme activate latte
```

If you want to use it with docker-compose, you can find a sample [docker-compose.yml file here](https://gist.github.com/HardeepAsrani/badd41d084658aec2781f07acf351c10).

If you have any questions or want to report an issue, please do it on [GitHub](https://github.com/HardeepAsrani/docker-wordpress-with-wp-cli/).

Please feel free to fork and use for your own projects, as this is forked from [conetix/docker-wordpress-wp-cli](https://github.com/conetix/docker-wordpress-wp-cli)
