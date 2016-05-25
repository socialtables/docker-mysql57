#  docker-mysql57

MySQL 5.7 - Social Tables Style

## Why

We like our MySQL 5.7 databases to:

- be enabled to use the utf8mb4 character set by default
- match the stock configuration that we don't alter on AWS RDS, which differs from the default MySQL image on docker hub
- match the customized parameter group we apply to our MySQL databases on AWS RDS

Also, it's nice when the MySQL container keeps its data outside of the container so that when you delete the container you don't delete all your data. This does that.

## Usage

```sh
docker-compose up -d
```
