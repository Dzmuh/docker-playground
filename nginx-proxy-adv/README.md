# nginx-proxy и проброс других сетей

В этом проекте я запущу службу `nginx-proxy` и выделю под неё сеть.
Имя сети обычно получается из названия папки, в которой размещается файл `docker-compose.yml`, в этом примере это `nginx-proxy-adv` и одноименное имя сети, т.е. имеем сеть `nginx-proxy-adv_proxy`.

В папке `nginx_service1` имеем файл `docker-compose.yml` который развернёт службу `nginx1` которую подцепим к сети `nginx-proxy-adv_proxy`, создав сеть `frontend` и пробросив её в сеть `nginx-proxy-adv_proxy`.

В общем, это конечно пипец, но он работает.

## docker-compose down и сеть nginx-proxy-adv_proxy

Если я выполню `docker-compose down` для `nginx-proxy-adv` не заглушив `nginx_service1`, то получим ошибку удаления сети и сеть `nginx-proxy-adv_proxy` останется висеть.
Будет висеть и после заглушки `nginx_service1` и нужно будет удалить её вручную или выполнить `docker-compose down` для `nginx-proxy-adv`.

## Ссылки для посмотреть

* [127.0.0.1.xip.io](http://127.0.0.1.xip.io/)
* [nginx1.127.0.0.1.xip.io](http://nginx1.127.0.0.1.xip.io/)

## Ссылки

* [nginx-proxy - GitHub](https://github.com/nginx-proxy/nginx-proxy)
