# Лабораторная 3.1 VPN

Выполнили: Аксеныч Семен, Самойлов Виктор

## Wireguard
Установка Wireguard

![-9MXIH6iT8Q](https://user-images.githubusercontent.com/87616197/161413408-95fdcabb-efaa-46cd-aba2-92c179c3659a.jpg)

Для создания конфигов установим инструмент easy-wg-quick (https://github.com/burghardt/easy-wg-quick)

![aGebzzzSHNI](https://user-images.githubusercontent.com/87616197/161416130-9ee1b291-9896-4784-861b-256ffe28c3ec.jpg)

Создадим с помощью него конфиги:

![k7grKjUZoLQ](https://user-images.githubusercontent.com/87616197/161416148-5f100dc5-bfb4-4a99-a886-d1c1d979ec41.jpg)

Полученный конфиг для сервера:

![HDmz48la7ao](https://user-images.githubusercontent.com/87616197/161416209-482fec7c-0239-48b1-9c40-dfd024f510eb.jpg)

Конфиг клиента:

![-8G_qy54acs](https://user-images.githubusercontent.com/87616197/161416214-3cea20e1-387e-4211-aa9f-eb50507b8dba.jpg)

Копируем конфиг в каталог wireguard и запускаем сервис:

![1KPet3EiJ6Q](https://user-images.githubusercontent.com/87616197/161416269-7444b099-a6c2-4202-9d61-bc4938e050f7.jpg)

Сохраняем на клиент конфиг и запускаем wireguard:

![BKm67IKsito](https://user-images.githubusercontent.com/87616197/161416315-e2a901ca-0741-4c9d-839a-22ce61c36667.jpg)

Проверяем, что всё работает на клиенте:

![aWwDSYE_bmk](https://user-images.githubusercontent.com/87616197/161416373-c3b48d83-d05a-4705-af2b-c315883e8cba.jpg)

![tl1niYlPPyE](https://user-images.githubusercontent.com/87616197/161416375-fe7353a8-b347-4326-b437-87b544c81c29.jpg)

Проверка на сервере:

![8E-O2qmKuFc](https://user-images.githubusercontent.com/87616197/161416393-a09036ab-d5d9-44b5-898f-9c34c3b477b5.jpg)


## IPSec/IKEv2

Скачиваем и запускаем скрипт (wget https://git.io/vpnsetup -qO vpn.sh && sudo sh vpn.sh):

![1fGAxXiANmM](https://user-images.githubusercontent.com/87616197/161416490-d1c93dde-f127-4bb2-b899-72d6e5bc4927.jpg)

Сохраняем на клиент файл vpnclient.p12, в тот же каталог скачиваем скрипт для автонастройки VPN подключения (https://github.com/hwdsl2/setup-ipsec-vpn/blob/master/extras/ikev2setup.sh) и запускаем его:

![vr8om9Nod8o](https://user-images.githubusercontent.com/87616197/161416802-c96c23b3-a559-42bb-905e-a67c74c13c72.jpg)

Проверка, что всё работает на клиенте:

![QM3yYQRhYSU](https://user-images.githubusercontent.com/87616197/161418493-9fcb20fa-e3b6-4863-9f6b-b31d5ac2cb80.jpg)

![zk49O_yw1zY](https://user-images.githubusercontent.com/87616197/161418494-861565be-5b40-4fe3-9b98-f79a65ed867b.jpg)







