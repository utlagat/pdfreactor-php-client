# PDFreactor Web Service PHP Client

Composer package for the official [RealObjects PDFreactor](https://www.pdfreactor.com) Web Service PHP client.

## Source

The file `src/PDFreactor.class.php` is the official PHP client from the RealObjects PDFreactor Web Service installation package, version **12.5.0**.

Downloaded from: https://www.pdfreactor.com/download/ (Web Service Clients)

**This package is not affiliated with RealObjects GmbH.** It repackages the official PHP client for convenient installation via Composer. PDFreactor is a commercial product — a valid license is required for production use. See https://www.pdfreactor.com for licensing information.

## Installation

```bash
composer require givo/pdfreactor-php-client
```

## Usage

```php
use com\realobjects\pdfreactor\webservice\client\PDFreactor;

$pdfReactor = new PDFreactor('http://localhost:9423/service/rest');

$config = ['document' => '<html><body><h1>Hello</h1></body></html>'];
$pdf = $pdfReactor->convertAsBinary($config);
```

## License

The PHP client file (`src/PDFreactor.class.php`) is copyright © RealObjects GmbH and subject to the [PDFreactor Software License Agreement](https://www.pdfreactor.com/product/license.html). See `LICENSE` for details.
