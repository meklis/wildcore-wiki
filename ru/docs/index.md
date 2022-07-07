## **WildcoreDMS** - система мониторинга, уведомлений и менеджмента устройств.

WildcoreDMS - это система направленная на диагностику, мониторинг и управление оборудованием. 
Основная цель - разгрузить инженеров/админов, дать возможность монтажнику провести диагностику в поле, 
а оператору сориентироваться в проблеме, этим сократив время реакции. 

### Базовый функционал
* Модульность - возможность подключать только необходимые компоненты   
* Работа в докер
* Легкая установка и обновление - с помощью специальной утилиты установка и обновление производится в несколько команд
* Легкая настройка системы
* HTTP RestAPI 
* Гибкое управление правами доступа пользователей, ограничение видимости групп устройств
* Логирование действий пользователей, работы с оборудованием
* Сбор метрик в Prometheus

### Поддерживаемые вендоры

* Dlink
* Edge-Core
* Huawei
* BDcom
* C-data
* Mikrotik
* ZTE       

Полный список поддерживаемого оборудования по моделям - [https://github.com/meklis/switcher-core/blob/master/docs/DEVICES.md](https://github.com/meklis/switcher-core/blob/master/docs/DEVICES.md)