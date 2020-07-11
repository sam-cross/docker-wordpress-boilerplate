# Super-Basic WordPress Boilerplate

This is a Docker boilerplate for a MySQL/PHP/Adminer/WordPress setup.

I'm new to Docker so if anything is wrong, please submit a PR (or just an Issue and I'll fix it later)!

## Initialising the Container

**YOU NEED TO DOWNLOAD WORDPRESS FIRST**

1. [Download WordPress](https://wordpress.org)
2. Extract the files _directly_ into the `wp/src` directory

## Running the Container

1. Run `docker-compose -f "docker-compose.yml" up -d --build` in the root directory of this repo.
2. ???
3. Profit!

-   Adminer is accessible on port `9000`: `http://localhost:9000`
-   WordPress is accessible on port `80`: `http://localhost`
-   The default MySQL database name is: `wp-practice`

## Big Warning

**DO NOT** use this in production without creating a new user specifically for WordPress. Currently, it uses the `root` user with the password `example`.
