Dockerfile for EC-CUBE 3.x with docker-compose
====

It's fork from https://github.com/nanasess/docker-ec-cube3

Windows User Notice: please change `End of Line Sequence` of  `wait-for-pgsql.sh` and `wait-for-mysql.sh`  to `LF` .

## What's this

Development environment for [EC-CUBE 3.x](https://github.com/EC-CUBE/ec-cube).

## How to Build Image

* git clone

```zsh
git clone https://github.com/codeyu/docker-ec-cube3.git
```

## Example Usage

```zsh
cd docker-ec-cube3
docker-compose up -d
```

Let's Access in Browser
  * Front End) ```http://localhost:8080```
  * Back End) ```http://localhost:8080/admin```
    * ID: admin / PW: password
  * MailCatcher) ```http://localhost:1080/```

### Use for MySQL

```zsh
docker-compose --project-name mysql -f docker-compose.yml -f docker-compose.mysql.yml up -d
```

### Cleanup

```zsh
docker-compose stop
docker-compose rm
```

----
* This software is released under the MIT License, see LICENSE.txt.



