# Добро пожаловать с наш  проект "Рога и копыта".

Он использует высокопроизводительный web сервер **Nginx**.
Для того что бы начать пользоваться им достачно:
1. Установить **Nginx** командой:
 * **Centos/RedHat**: yum install nginx
 * **Debian/Ubuntu**: apt install nginx
2. Собрать вручную, предварительно скачав с сайта [nginx.org](http://hg.nginx.org/nginx.org)
3. Скопировать файл **nginx.conf** и заменить базовый.
Для того, что бы у вас заработало архивирование необходимо заменить блок:
```
        gzip on;

        # gzip_vary on;
        # gzip_proxied any;
        # gzip_comp_level 6;
        # gzip_buffers 16 8k;
        # gzip_http_version 1.1;
        # gzip_types text/plain text/css application/json application/javascript text/xml application/xml application/xml+rss text/javascript;
```
На:
```
	gzip on;

        gzip_vary on;
        gzip_proxied any;
        gzip_comp_level 6;
        gzip_buffers 16 8k;
        gzip_http_version 1.1;
        gzip_types text/plain text/css application/json application/javascript text/xml application/xml application/xml+rss text/javascript;
```

# Welcome to our project "Horns and Hooves".
It uses a high performance web server **Nginx**.
In order to start using it, it is enough:
1. Install **Nginx** with the command:
  * **Centos/RedHat**: yum install nginx
  * **Debian/Ubuntu**: apt install nginx
2. Build manually, after downloading from the site [nginx.org](http://hg.nginx.org/nginx.org)
3. Copy the *nginx.conf* file and replace the base one.
In order for archiving to work for you, you need to replace the block:
```
 	 gzip on;

        # gzip_vary on;
        # gzip_proxied any;
        # gzip_comp_level 6;
        # gzip_buffers 16 8k;
        # gzip_http_version 1.1;
        # gzip_types text/plain text/css application/json application/javascript text/xml application/xml application/xml+rss text/javascript;
```
On:
```
  	gzip on;

        gzip_vary on;
        gzip_proxied any;
        gzip_comp_level 6;
        gzip_buffers 16 8k;
        gzip_http_version 1.1;
        gzip_types text/plain text/css application/json application/javascript text/xml application/xml application/xml+rss text/javascript;
``` 
