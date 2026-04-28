# UniSms Library

The official SDK for UniSMS https://unismsapi.com/ for sending and retrieving SMS messages.

This is Vanilla PHP.

## Send a message


```php
require_once './UniSms.php';

$secret_key = "sk_XXXXXXXXXXXXXXXXXXXXXXXXX";

$client = new UniSms($secret_key);
$client->recipient = "+63912345678";
$client->content = "Hello world";
$client->send();
```

## Send a message with your custom Sender id: MyBusiness

```php
require_once './UniSms.php';

$secret_key = "sk_XXXXXXXXXXXXXXXXXXXXXXXXX";

$client = new UniSms($secret_key);
$client->recipient = "+63912345678";
$client->content = "Hello world";
$client->sender_id = "MyBusiness";

$client->send();
```

## Get a message


```php
require_once './UniSms.php';

$secret_key = "sk_XXXXXXXXXXXXXXXXXXXXXXXXX";
$client = new UniSms($secret_key);
$client->get("msg_b788f2bf-5816-47c1-8eb0-f018a699d7bc");
```
