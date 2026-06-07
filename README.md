# FromGram для Android

Это исходный код клиента для [FromGram](https://github.com/fromchat-messenger/fromgram), неофициального кастомного сервера Telegram.

## Компиляция

1. Клонируйте и импортируйте проект в [Android Studio](https://developer.android.com/studio).
2. Откройте [`ConnectionsManager.cpp`](TMessagesProj/jni/tgnet/ConnectionsManager.cpp) 
   и в `ConnectionsManager::initDatacenters()` замените IP и порт на ваши.
3. Откройте [`Datacenter.cpp`](TMessagesProj/jni/tgnet/Datacenter.cpp) и в 
   `*Datacenter::decodeSimpleConfig` замените публичный ключ на ваш.
4. Запустите конфигурацию `TMessagesProj_App` в Android Studio.
5. Готово!

## Документация

Telegram API: https://core.telegram.org/api

MTProto: https://core.telegram.org/mtproto

## Лицензия

GPLv2. При распространении вы тоже должны опубликовать свой исходный код.
