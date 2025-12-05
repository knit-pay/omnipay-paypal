# Omnipay: PayPal

**PayPal driver for the Omnipay PHP payment processing library**

[![Latest Stable Version](http://poser.pugx.org/knit-pay/omnipay-paypal/v)](https://packagist.org/packages/knit-pay/omnipay-paypal) [![Total Downloads](http://poser.pugx.org/knit-pay/omnipay-paypal/downloads)](https://packagist.org/packages/knit-pay/omnipay-paypal) [![Latest Unstable Version](http://poser.pugx.org/knit-pay/omnipay-paypal/v/unstable)](https://packagist.org/packages/knit-pay/omnipay-paypal) [![License](http://poser.pugx.org/knit-pay/omnipay-paypal/license)](https://packagist.org/packages/knit-pay/omnipay-paypal) [![PHP Version Require](http://poser.pugx.org/knit-pay/omnipay-paypal/require/php)](https://packagist.org/packages/knit-pay/omnipay-paypal)

[Omnipay](https://github.com/thephpleague/omnipay) is a framework agnostic, multi-gateway payment
processing library for PHP. This package implements PayPal support for Omnipay.

## Installation

Omnipay is installed via [Composer](http://getcomposer.org/). To install, simply require `league/omnipay` and `knit-pay/omnipay-paypal` with Composer:

```
composer require league/omnipay knit-pay/omnipay-paypal
```


## Basic Usage

The following gateways are provided by this package:

* PayPal_Rest (Paypal Rest API)
* PayPal_Express (PayPal Express Checkout)
* PayPal_ExpressInContext (PayPal Express In-Context Checkout)
* PayPal_Pro (PayPal Website Payments Pro)

For general usage instructions, please see the main [Omnipay](https://github.com/thephpleague/omnipay)
repository.

## Quirks

The transaction reference obtained from the purchase() response can't be used to refund a purchase. The transaction reference from the completePurchase() response is the one that should be used.

## Out Of Scope

Omnipay does not cover recurring payments or billing agreements, and so those features are not included in this package.

## Support

If you are having general issues with Omnipay, we suggest posting on
[Stack Overflow](http://stackoverflow.com/). Be sure to add the
[omnipay tag](http://stackoverflow.com/questions/tagged/omnipay) so it can be easily found.

If you want to keep up to date with release anouncements, discuss ideas for the project,
or ask more detailed questions, there is also a [mailing list](https://groups.google.com/forum/#!forum/omnipay) which
you can subscribe to.

If you believe you have found a bug, please report it using the [GitHub issue tracker](https://github.com/knit-pay/omnipay-paypal/issues),
or better yet, fork the library and submit a pull request.
