# Yandex-tts-speechkit-FIX
# Исправленный кастом компонент для TTS Yandex для Home Assistant

Работает с новыми АПИ Ключами полученными https://console.cloud.yandex.ru/
Этот ключ можно получить бесплатно на 60 дней. (Нужна карта виза. мастеркард ) Дальше платно.
Не работает со старыми ключами.

Для настройки:
Создайте если еще нет папку custom_components рядом с вашим конфигурационным файлом yaml
В ней создайте папку yandextts
Скопируйте файлы из репозитория что бы они лежали так:
\custom_components\yandextts\__init__.py
\custom_components\yandextts\manifest.json
\custom_components\yandextts\tts.py

Пример настройки 
  - platform: yandextts
    api_key: *******************Pgm9ibWdjPc********
    base_url: https://user.duckdns.org:8123
    language: 'ru-RU'
    codec: oggopus
    voice: oksana
    
К выводу не доступен mp3. Ограничение у апи.
Возвращает только oggopus или lpcm.
Не используйте codec: mp3.
Используйте 
codec: oggopus 
или
codec: lpcm.
Не используйте эмоции.
Остальные поции не проверял.    
    
