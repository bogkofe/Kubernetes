## Домашнее задание к занятию «Управление доступом»

# Задание 1
- Создал  SSL-сертификат для подключения к кластеру для пользователя sagirov настроил конфигурационный файл kubectl для подключения
![image](https://github.com/bogkofe/Kubernetes/blob/master/2.4/files/1.png)

- Создал роль и с необходимыми правами пользователя
[Ссылка на role.yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.4/z1/role.yaml)

- Привязал роль к пользователю sagirov
[Ссылка на rolebinding.yaml файл](https://github.com/bogkofe/Kubernetes/blob/master/2.4/z1/rolebinding.yaml)

- Заранее были подняты поды и сервисы. Как и ожидалось, к информации подов доступ есть, к остальному нет
![image](https://github.com/bogkofe/Kubernetes/blob/master/2.4/files/2.png)
