# Etsy Provider for OAuth 1.0 Client

[![Latest Stable Version](https://img.shields.io/packagist/v/gentor/oauth1-etsy.svg)](https://packagist.org/packages/gentor/oauth1-etsy)
[![License](https://img.shields.io/packagist/l/gentor/oauth1-etsy.svg)](https://github.com/gentor/oauth1-etsy/blob/master/LICENSE)
[![Total Downloads](https://img.shields.io/packagist/dt/gentor/oauth1-etsy.svg?maxAge=2592000)](https://packagist.org/packages/gentor/oauth1-etsy)

This package provides Etsy API OAuth 1.0 support for the PHP League's [OAuth 1.0 Client](https://github.com/thephpleague/oauth1-client).

## Installation

Via Composer

```shell
$ composer require gentor/oauth1-etsy
```

## Usage

Usage is the same as The League's OAuth client, using `Gentor\OAuth1Etsy\Client\Server\Etsy` as the provider.

```php
$server = new Gentor\OAuth1Etsy\Client\Server\Etsy([
    'identifier'   	=> 'your-client-id',
    'secret'       	=> 'your-client-secret',
    'scope'			=> '', //See Etsy documentation for the full list of permission scopes
    'callback_uri' 	=> 'http://callback.url/callback'
]);
```

### Permission Scopes
See the Etsy documentation for [Permission Scopes](https://www.etsy.com/developers/documentation/getting_started/oauth#section_permission_scopes)


## License

The MIT License (MIT). Please see [License File](https://github.com/thephpleague/oauth1-client/blob/master/LICENSE) for more information.
