# Lottery-Poetry-Sixty-Jiazi

Lottery-Poetry-Sixty-Jiazi is the data of Lottery-Poetry-Engine.

## Requirement

 - PHP >=5.4

## Installing via Composer

The recommended way to install Lottery-Poetry-Sixty-Jiazi is through Composer.

```bash
# Install Composer
curl -sS https://getcomposer.org/installer | php
```

Next, update your project's composer.json file to include Lottery-Poetry-Sixty-Jiazi:

```json
{
    "require": {
        "destinylab/lottery-poetry-sixty-jiazi": "dev-master"
    }
}
```

## Usage

```php
<?php

require_once 'vendor/autoload.php';

$suit = new DestinyLab\LotteryPoetry\SixtyJiazi([__DIR__.'/resources'], 'yml');
$engine = new DestinyLab\LotteryPoetry\Engine($suit);

// get contents
$engine->draw();

// get only key
$engine->draw(true);
```

## License

MIT