# OpenVPN gateway

Файлы настроек шлюза openvpn с пушем DNS cloudflare клиенту. 

В файле [conf-server](conf-server) настройки, которые необходимо выполнить на сервере (SElinux, enable forwarding kernel)

В файле [firewalld-rules](firewalld-rules) список правил, которые нужно сделать в firewalld (здесь **tun0** внутренний интерфейс, который
создает openvpn, а **ens3** внешний интерфейс на который необходимо пробрасывать порты).

Файл [server.conf](server.conf) - конфигурация openvpn сервера. 

Файл [client-config.ovpn](client-config.ovpn) конфигурация для клиента.

В файлах настроек при наличии параметров вида %name% необходимо заменить их на свои.
