[![hacs_badge](https://img.shields.io/badge/HACS-Custom-orange.svg?style=for-the-badge)](https://github.com/custom-components/hacs)

# Yandex-tts-speechkit-FIX
# Исправленный кастом компонент TTS Yandex для Home Assistant


Работает с новыми API Ключами полученными https://console.cloud.yandex.ru/
Этот ключ можно получить бесплатно на 60 дней. (Нужна карта Visa или Mastercard ) Дальше только платное исаользование.
Не работает со старыми ключами.


Пример настройки 

  - platform: yandextts
  
    api_key: ***************************
    
    
    language: 'ru-RU'
    
    codec: lpcm
    
    voice: oksana
    
Используйте codec: lpcm.

К выводу не доступен mp3. Ограничение по API.
Не используйте codec: mp3.

Не используйте codec: oggopus 
Начиная с 115.4 он не обрабатывается в ха без ошибок.

Не используйте эмоции.
Остальные поции не проверены на работоспособность.

# Установка через HACS
Вставьте ссылку https://github.com/tayanov/Yandex-tts-speechkit-FIX в раздел CUSTOM REPOSITORIES в HACS
    
