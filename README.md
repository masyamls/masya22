Создали vm.

ввели команды:
sudo yum install wget
sudo yum install curl
sudo yum install git

![image](https://github.com/user-attachments/assets/30fe6ddc-fdda-449c-a272-1de063dbe0ac)

![image](https://github.com/user-attachments/assets/7f5b7332-cb15-4103-9b80-2ef2e5a0b4c6)

![image](https://github.com/user-attachments/assets/35d8f5a1-09be-4eb3-aead-0278f9887fb5)


Следущая команда была sudo yum install tar

![image](https://github.com/user-attachments/assets/cdb100c0-e85e-4b76-8b95-e9a2f0befd07)

установка: sudo yum install chromy

![image](https://github.com/user-attachments/assets/6b4799b6-f86c-4351-8cf6-56ea966bde75)

включение в автозагрузку: systemctl enable chronyd

![image](https://github.com/user-attachments/assets/8d5127a7-6ac3-4316-8916-446b51d3c36f)

запуск службы:systemctl start chronyd

![image](https://github.com/user-attachments/assets/f199c287-b70b-4a50-ac15-a56b115e19aa)

проверяю гетинфорс (getenforce) командой getenforce. получила в ответ:
Enforcing. Следовательно исправляем ошибку

5.пункт
скачиваем Prometheus. 3.3.0 / 2025-04-15 версия

команда: wget https://github.com/prometheus/prometheus/releases/download/v3.3.0/prometheus-3.3.0.linux-amd64.tar.gz

![image](https://github.com/user-attachments/assets/227a1772-9497-466b-bf83-680baa259137)

![image](https://github.com/user-attachments/assets/45a2ec38-4512-4acf-852a-bce42b7006a0)

создадим каталоги для промитьюса: mkdir /etc/prometheus /var/lib/prometheus

распаковали архив: tar xvf prometheus-3.3.0.linux-amd64.tar.gz

![image](https://github.com/user-attachments/assets/c2c082be-8449-4d00-889a-4d4b3f3d8d71)

перешли в директорию: cd prometheus-3.3.0.linux-amd64

![image](https://github.com/user-attachments/assets/6c0b0663-327a-45b3-bad8-c8dca9b3a835)

pwd
![image](https://github.com/user-attachments/assets/0743b4aa-a79d-4c44-b2dd-c8370b4c5453)

Раскидали по папкам системы файлы прометеуса: cp prometheus promtool /usr/local/bin/ и cp prometheus.yml /etc/prometheus 

![image](https://github.com/user-attachments/assets/ba928505-f0b2-4812-a9ca-a8ab4a432846)

возвращаемся в родительский каталог, удаляем распакованную папку и архив

![image](https://github.com/user-attachments/assets/b4117549-ff10-4946-816f-e581d1686a50)

pwd

![image](https://github.com/user-attachments/assets/6e5e8e18-b088-4a4c-b876-782b16d11e4f)

ls -l

![image](https://github.com/user-attachments/assets/042d700c-78b7-422e-a5ff-df780d0276b5)

