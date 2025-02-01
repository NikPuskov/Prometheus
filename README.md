# Prometheus

Стенд на Vagrant (бокс ubuntu/jammy64) с прописанной установкой Docker, созданием Docker-образа Prometheus и запуском Docker-контейнеров Prometheus, Node_Exporter, Grafana

(Vagrantfile, Dockerfile и конфиг Prometheus прилагаются)

`vagrant up`

`vagrant ssh`

Смотрим ip адрес

![Image alt](https://github.com/NikPuskov/Prometheus/blob/main/grafana1.jpg)

Настройки Grafana:

a) В браузере ip_address:3000 -> admin/admin (в моём случае ip адрес 192.168.0.188)

b) connections -> data sources -> add new data source -> prometheus -> ip_address:9090 -> save and test

c) dashboards -> import dashboard -> 1860 -> load

![Image alt](https://github.com/NikPuskov/Prometheus/blob/main/grafana.jpg)
