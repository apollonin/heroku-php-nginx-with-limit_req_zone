# heroku-php-nginx-with-limit_req_zone

**heroku.conf.php** file was copied from [original](https://github.com/heroku/heroku-buildpack-php/blob/master/conf/nginx/heroku.conf.php) repo.

with additional line:

```
limit_req_zone $binary_remote_addr zone=login:10m rate=2r/s;
```
