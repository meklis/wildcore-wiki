## Передмова
Якщо в процесі роботи ви зіткнулися з проблемами в роботі з агентом, переконайтеся, що ви використовуєте актуальну версію ПЗ.

### Вирішення майже всіх проблем
Можливо, що в якомусь із оновлень частина ресурсів не була оновлена, кеші не були очищені і т.д.
Виконайте такі команди, щоб виключити можливі проблеми: 
```shell
cd /opt/wildcore-dms 
sudo docker compose down --remove-orphans
sudo docker compose up -d --build 
# Тут потрібно почекати деякий час, поки запустяться всі контейнери. Якщо використовується HDD – збільште час вдвічі
sleep 10 
wca cache:flush
wca cache:redis:flush-all
```

## Звернення в підтримку

Перед зверненням:    

1. **Переконайтесь, що використовуєте актуальну версію агента и утиліти wca-tool**
2. Виконайте команди описані в ["Вирішення майже всіх проблем"](#_2)      
3. Переконайтесь, що у сервера є стабильний доступ до обладнання (наприклад, ping і snmpwalk)     

Якщо кроки вище не вирішили проблему, при зверненні намагайтеся максимально описати дії, які викликають проблему, вкажіть:   

* Характеристики системи, на якій працює ПЗ
* Роль користувача під яким з'являється помилка;
* Які права надані цій групі користувачів;
* На якому обладнанні (якщо це обладнання) виникли проблеми. Бажано також надати висновок команди `wca switcher-core:call IP_УСТРОЙСТВА system`;
* Надати скрини
* Описати що саме не так, навіть якщо це очевидно для вас (але кожен розуміє по-своєму))))   
* Які доступи до обладнання надали (комуніті - RO або RW, логін/пароль як користувач або адміністратор)   

[Контакти підтримки](/ru/contact/contacts/#_2)
