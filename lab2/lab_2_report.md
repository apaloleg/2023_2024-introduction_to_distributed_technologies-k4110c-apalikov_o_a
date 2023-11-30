University: [ITMO University](https://itmo.ru/ru/)
Faculty: [FICT](https://fict.itmo.ru)
Course: [Introduction to distributed technologies](https://github.com/itmo-ict-faculty/introduction-to-distributed-technologies)
Year: 2023/2024
Group: K4110c
Author: Apalikov Oleg Aleksandrovich
Lab: Lab2
Date of create: 13.10.2023
Date of finished:

1. Запускаем Minikube
![1. Запускаем MiniKube](../screenshots/lab1_img_1.png)

2. Создаем Deployment
![2. Создаем Deployment](../screenshots/lab2_img_1.png)

3. Создаем Service
![3. Создаем Service](../screenshots/lab2_img_2.png)

4. Деплоим deployment и service
```
kubectl apply -f lab2/react-deployment.yml
```
![4. Deploy](../screenshots/lab2_img_3.png)

5. Прокидываем порт, открываем приложение
```
minikube kubectl -- port-forward service/react 3000:3000
```
![5. App](../screenshots/lab2_img_4.png)

Значения переменных REACT_APP_USERNAME и REACT_APP_COMPANY_NAME соответствуют переданным. Название и IP пода могут меняться в зависимости от того, на какой под уйдет запрос.


Логи пода:
![6. Логи пода](../screenshots/lab2_img_5.png)

Схема:
![7. Схема](../screenshots/lab2_img_6.png)
