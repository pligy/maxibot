# ApiHelper
## class maxibot.apihelper.Api(token)
Клиент для рабты с api MAX  
**Параметры:**
* **client** (`str`) - тип сообщения  

**Методы:**
* **get_my_info** - Получение информации о текущем боте  
* **get_updates** (`allowed_updates`, `extra`) - Получение новых обновлений от API через лонгполлинг  
    * `allowed_updates` - Список типов обновлений, которые нужно получать  
    * `extra` - Дополнительные параметры запроса  
* **get_message** (`msg_id`) - Получение сообщений по `msg_id`  
    * `msg_id` - Уникальный идентификатор сообщения  
* **send_message** (`chat_id`, `msg_id`, `text`, `method`, `attachments`, `parse_mode`, `notify`) - Отправка/удаление/обновление сообщение в чате  
    * `chat_id` - Уникальный идентификатор чата  
    * `msg_id` - Уникальный идентификатор сообщения  
    * `text` - Текст сообщения  
    * `method` - HTTP метод для запроса  
    * `attachments` - Вложения сообщения  
    * `parse_mode` - Формат текста сообщения (`Markdown`, `HTML`)  
    * `notify` - Флаг необходимости звукового уведомления  
* **answer_callback**(`callback_id`,`text`,`notification`, `attachments`, `link`, `notify`, `format`)  
    * `callback_id` - Уникальный идентификатор callback-запроса
    * `text` - Новый текст сообщения. Если указан, сообщение будет обновлено  
    * `notification` - Текст всплывающего уведомления для пользователя  
    * `attachments` - Новые вложения сообщения  
    * `link` - Ссылка на сообщение для reply/forward формата  
    * `notify` - Отправлять ли системное уведомление в чат об изменении сообщения  
    * `format` - Формат текста сообщения (`Markdown`, `HTML`)  