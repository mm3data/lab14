#  Настройка протоколов CDP, LLDP и NTP  

## Топология  
<img width="740" height="111" alt="image" src="https://github.com/user-attachments/assets/a0b6be56-ddb2-4e21-bd9d-81f3a900e4a5" />  

##  Таблица маршрутизации  

Утсройство | Интерфейс | IP-адрес | Маска подсети | Шлюз по умолчанию 
-- | -- | -- | -- | --  
R1 | Loopback1 | 172.16.1.1 | 255.255.255.0 | ---  
-- | G0/0/1 | 10.22.0.1 | 255.255.255.0 | ---  
S1 | SVI VLAN1 |10.22.0.2 | 255.255.255.0 | ---  
SS2 | SVI VLAN2 | 10.22.0.3 | 255.255.255.0 | ---  

##  Задачи  
* Создание сети и настройка основных параметров устройства  
* Обнаружение сетевых ресурсов с помощью протокола CDP  
* Обнаружение сетевых ресурсов с помощью протокола LLDP  
* Настройка и проверка  

## Настройка базовых параметров маршрутизатора  

<img width="654" height="748" alt="image" src="https://github.com/user-attachments/assets/81841f3e-04d6-4e70-bf02-ccf0aa895788" />      

<img width="330" height="134" alt="image" src="https://github.com/user-attachments/assets/4a5653db-9083-4e22-91e2-31550c2ddbc6" />    

## Настройка базовых параметров коммутатора  
* S1

<img width="690" height="666" alt="image" src="https://github.com/user-attachments/assets/b7ef11f6-7f10-46be-950a-47cf5d0fa1af" />    

<img width="698" height="256" alt="image" src="https://github.com/user-attachments/assets/780f066d-d028-43b9-baad-562b2e0899a0" />    

* S2

<img width="669" height="666" alt="image" src="https://github.com/user-attachments/assets/436b9283-c9ac-4fba-8c8f-97bd0d62aa2f" />   
<img width="347" height="106" alt="image" src="https://github.com/user-attachments/assets/3345c9a0-245d-440e-948b-bb9732808f35" />   

## Обнаружение сетевых ресурсов с помощью протокола CDP  

<img width="800" height="631" alt="image" src="https://github.com/user-attachments/assets/ac2ac1bf-f151-4324-9713-81920ed40d95" />  

_Сколько интерфейсов участвует в объявлениях CDP? Какие из них активны?_  

* G0/0/1  
_Какая версия IOS используется на  S1?_

* Version 15.0(2)SE4

<img width="604" height="273" alt="image" src="https://github.com/user-attachments/assets/e4db3578-527e-43fa-a34f-f831cabba727" />  

## Настройка SVI для VLAN 1 на S1 и S2  

<img width="615" height="353" alt="image" src="https://github.com/user-attachments/assets/f8231ffa-59dc-4222-bb37-ebb37368cbfb" />  
<img width="610" height="336" alt="image" src="https://github.com/user-attachments/assets/2f1397f3-7586-464f-957c-96d7a9ca5013" />

## На R1 show cdp entry S1   
_Какие дополнительные сведения доступны теперь?_   
<img width="612" height="116" alt="image" src="https://github.com/user-attachments/assets/803da813-d1cb-43c1-ba6f-1c34e2137b27" />  
ip-адрес 10.22.0.2  

## Отключаем CDP на всех устройствах  
<img width="1813" height="103" alt="image" src="https://github.com/user-attachments/assets/8ca4caed-7c66-4d07-a3a2-72fa4c0f0173" />  

## LLDP  
<img width="599" height="488" alt="image" src="https://github.com/user-attachments/assets/88c2aac6-96d1-4e0e-a830-fab0bef85907" />   

_Что такое chassis ID  для коммутатора?_  
Уникальный идентификатор устройства, который используеться в протоколе LLDP и CDP


<img width="609" height="452" alt="image" src="https://github.com/user-attachments/assets/3c72c935-723f-47a5-9a1b-0207d01e9553" />  
<img width="912" height="806" alt="image" src="https://github.com/user-attachments/assets/328fadf4-8cbb-4ce2-b063-1108e78adf63" />  
<img width="822" height="577" alt="image" src="https://github.com/user-attachments/assets/65f7b00f-1472-4b1c-8c93-f695880798f1" />

## NTP  

<img width="264" height="53" alt="image" src="https://github.com/user-attachments/assets/52c07211-e343-446a-98df-6b8b6414f887" />    

<img width="283" height="97" alt="image" src="https://github.com/user-attachments/assets/ffae1c0b-bca0-419d-a6c4-f4be1c2fc57a" />  



<img width="611" height="483" alt="image" src="https://github.com/user-attachments/assets/ec0e60a7-35aa-4c59-b336-168371303f21" />  

<img width="682" height="254" alt="image" src="https://github.com/user-attachments/assets/d7c4fc10-3852-4893-a24a-07015c1563f4" /> 

<img width="887" height="199" alt="image" src="https://github.com/user-attachments/assets/195b4b45-06c5-4af1-b742-82739e2e4483" />    

<img width="297" height="128" alt="image" src="https://github.com/user-attachments/assets/9663a6bb-f7cd-43aa-a131-a2bfb41bcad8" />   

<img width="287" height="144" alt="image" src="https://github.com/user-attachments/assets/0adaf0a9-2257-4d51-ad3d-d860bd38d5d0" />    

<img width="298" height="235" alt="image" src="https://github.com/user-attachments/assets/324201be-9c39-46ac-87ab-f65a2965dc7b" />  

<img width="464" height="131" alt="image" src="https://github.com/user-attachments/assets/e2878dc1-e235-48d2-8a1d-7d8e1c7bb738" />  
















