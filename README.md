# Yandex-GPT-PHP
Класс для общения с Yandex GPT в PHP

1. Получите OAuth токен Яндекса и вставьте его в CLIENT_AUTH скрипта ([https://cloud.yandex.ru/ru/docs/iam/operations/iam-token/create](https://cloud.yandex.ru/ru/docs/iam/operations/iam-token/create#api_1))
2. Получите идентификатор каталога, на который у вашего аккаунта есть роль ai.languageModels.user или выше b вставьте его в X_FOLDER_ID скрипта (https://cloud.yandex.ru/ru/docs/resource-manager/operations/folder/get-id#console_1)
   
Использование:
```
require __DIR__ . '/yachat.php';
use yachat\YaChat;

$ya = yachat::getInstance();
echo $ya::answer('Привет');
```

