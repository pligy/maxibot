# Poling
## class maxibot.core.network.Polling(api, allowed_updates)
Объект, представляющий сообщение  
MAX API документация: https://dev.max.ru/docs-api/objects/Message  
**Параметры:**
* **token** (`str`) - Токен бота  
* **allowed_updates** (`str`) - Разрешённые события  

**Методы:**
* **stop** - Метод остановки поллинга  
* **loop** (`handler`) - Метод запуска поллинга  
    * **handler** - Функция, обрабатывающая полученные обновления API MAX
* **_get_updates** - Метод получения обновлений по боту из API MAX  
