# 10.1 Keepalived/vrrp

# Домашнее задание к занятию "`Keepalived/vrrp`" - `Колобов Михаил`

### Задание 1
Разверните топологию из лекции и выполните установку и настройку сервиса Keepalived. 

```
vrrp_instance test {
state "name_mode"
interface "name_interface"
virtual_router_id "number id"
priority "number priority"
advert_int "number advert"
authentication {
auth_type "auth type"
auth_pass "password"
}
unicast_peer {
"ip address host"
}
virtual_ipaddress {
"ip address host" dev "interface" label "interface":vip
}
}
```

*В качестве решения предоставьте:*   
*- рабочую конфигурацию обеих нод, оформленную как блок кода в вашем md-файле;*   
*- скриншоты статуса сервисов, на которых видно, что одна нода перешла в MASTER, а вторая в BACKUP state.*   

#### Ответ

1. ![01-01](https://github.com/Mikhail-2023/Keepalived_vrrp/blob/main/screen/01-01.PNG)
2. ![01-02](https://github.com/Mikhail-2023/Keepalived_vrrp/blob/main/screen/01-02.PNG)
3. ![01-03](https://github.com/Mikhail-2023/Keepalived_vrrp/blob/main/screen/01-03.PNG)
4. ![01-04](https://github.com/Mikhail-2023/Keepalived_vrrp/blob/main/screen/01-04.PNG)
5. ![01-05](https://github.com/Mikhail-2023/Keepalived_vrrp/blob/main/screen/01-05.PNG)
6. ![01-06](https://github.com/Mikhail-2023/Keepalived_vrrp/blob/main/screen/01-06.PNG)
