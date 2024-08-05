## Домашнее задание к занятию «Конфигурация приложений»

# Задание 1
- Создал  Deployment приложения, состоящего из контейнеров контейнеров nginx и multitool
[Ссылка на deployment.yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.3/z1/deployment.yaml)

- Решил проблему с портами с моиощью  ConfigMap
[Ссылка на configmap1.yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.3/z1/configmap1.yaml)

- После исправления под стартовал и оба контейнера работают
![image](https://github.com/bogkofe/Kubernetes/blob/master/2.3/files/1.png)

- Создал простую веб страницу и подключил ее к Nginx с помощью ConfigMap
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.3/z1/configmap2.yaml)

- Так же создал service для nginx
[Ссылка на yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.3/z1/service.yaml)


- Демонстрация, что все работает. Перешел по адресу и получил ожидаемый вывод
![image](https://github.com/bogkofe/Kubernetes/blob/master/2.3/files/2.png)


# Задание 2 

- Создал Deployment приложения, состоящего из Nginx.
[Ссылка на deployment.yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.3/z2/deployment.yaml)

- Создал веб-страницу и подключил её как ConfigMap к приложению
[Ссылка на configmap.yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.3/z2/configmap.yaml)

- Выпустил самоподписанный сертификат с помощью openssl
![image](https://github.com/bogkofe/Kubernetes/blob/master/2.3/files/3.png)

- Создал Secret для использования сертификата
[Ссылка на secret.yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.3/z2/secret.yaml)

- Создал Ingress и необходимый Service, подключил к нему SSL
[Ссылка на service.yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.3/z2/service.yaml)

[Ссылка на ingress.yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.3/z2/ingres.yaml)

- Демонстрация, что есть доступ к приложению по HTTPS. В доверенный сертификат не стал добавлять.
![image](https://github.com/bogkofe/Kubernetes/blob/master/2.3/files/4.png)

