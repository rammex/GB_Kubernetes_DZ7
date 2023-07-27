# Домашнее задание к уроку 7 - Продвинутые абстракции Kubernetes

Разверните в кластере сервер системy мониторинга Prometheus.

Создайте StatefulSet для Prometheus сервера из образа prom/prometheus:v2.19.2 с одной репликой

В нем должнен быть описан порт 9090 TCP volumeClaimTemplate - ReadWriteOnce, 5Gi, подключенный по пути /prometheus Подключение конфигмапа с настройками выше по пути /etc/prometheus

Так же укажите поле serviceAccount: prometheus на одном уровне с containers, initContainers, volumes См пример с rabbitmq из материалов лекции.

Проверьте что при обращении из браузера на белый IP вы видите открывшееся приложение Prometheus







