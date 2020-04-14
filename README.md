#  Docker Hashtopolis Server

## Configuration

Update `docker-compose.yml` and edit the following environement vars:
- `MYSQL_DATABASE`(default value is `hashtopolis_db`)
- `MYSQL_USER`(default value is `hashtopolis`)
- `MYSQL_PASSWORD`(default value is `mysql_password`)

As recommended in the [hashtopolis server prerequisites](https://github.com/s3inlc/hashtopolis/wiki/Server-Prerequisites), you may want to edit some Apache/PHP parameters in order to accommodate your intended usage.


## Install

```bash
docker-compose up -d
```

## Usage

Once installation is complete, use `mysql` for `Server Hostname`, let the default mysql port 3306 and add your custom parameters to setup the database connection.

![](https://github.com/zteeed/docker-hashtopolis-server/blob/master/.pics/hashtopolis_install.png)
