# Yii2 Mailgun mailer

Install through Composer:

```
composer require understeam/yii2-mailgun:^0.1 --prefer-dist
```

Configure:

```php
...
'mailer' => [
    'class' => 'understeam\mailgun\Mailer',
    'domain' => 'domain.com',
    'apiKey' => 'api-key',
],
...
```

Use:

```php
$message = Yii::$app->mailer->compose('@common/mail/signup', ['user' => $user]);
$message->send();
```

