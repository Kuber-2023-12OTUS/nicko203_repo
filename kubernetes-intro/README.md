# Домашнее задание 1.


На виртуальных машинах под управлением гипервизора KVM создан кластер Kubernetes в составе трёх управляющих нод и двух рабочих нод:

![nodes_list.png](images/nodes_list.png)

Командой kubectl `apply -f ./`  создаётся namespace `homework`   и  pod `homework01`, содержащий сервис nginx:


![create_pod.png](images/create_pod.png)


В результате общий список подов выглядит следующим образом:


![pods_list.png](images/pods_list.png)


Созданный под расположен на ноде `worknode02.sysad.su` и имеет адрес `10.244.3.2`

Проверить работу сервиса nginx можно командой `curl http://10.244.3.2:8000`


![check_service.png](images/check_service.png)





