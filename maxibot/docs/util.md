# Util
## class maxibot.util
Модуль, предоставляющий набор технических вспомагательных функций  
**Методы:**
* **is_command** (`text`) - Проверка, является ли `text` командой  
* **extract_command** (`text`) - Получение команды из текста `text` сообщения  
* **is_pil_image** (`var`) - Проверка, является ли `var` объектом типа `PIL.Image.Image`  
* **pil_image_to_bytes** (`image`, `extension`, `quality`) - Получение байткода из объекта типа, `PIL.Image.Image`  
    * **image** - объект типа `PIL.Image.Image`
    * **extension** - Разрешение изображения
    * **quality** - Качество изображения
* **get_text** (`media`) - Метод получения текста из `media`  
* **get_parce_mode** (`media`) - Метод получения типа формата из `media`  