# zeroCDN
![alt text](https://imgur.com/AraCZ0M.png)



zeroCDN is a powerful Layer7 Protection which is written in PHP.

**zero** detects all kind of harmful HTTP Traffic and blocks them accordingly. It can detect almost every single Bypass-Method using simple Methods that check for Parameters like UA, IP & ASN.

## Installation

Put the **fp.php** into the root of your directory and include it in your main core/index via:

```php
require_once 'fp.php';
```
After that you configure Cloudflare for your Webserver and set the Riskmode to "Medium". (Optional)
Using Cloudflare you can also use their invisible JS-Detection.

If you are using the Customer-Version, you have to build a compiled Version using the Source to configurate your Sitekeys. (reCaptcha)

## Features

It detects many Type of Attacks, for example:

* HTTP-GETFLOOD
* HTTP-POSTFLOOD
* HTTP-RANDOM
* SOCKET-FLOOD
* GET
* POST
* CF-BYPASS
* UDP Attacks
* SYNFLOOD
* BOT-REQ

... & many more! If we find a new bypass we will update our Firewall accordingly to be protected.

Some of our current Features:

* Ratelimiting
* reCaptcha (only in the paid version)
* Instant Notification if malicious Attack is coming towards your Webserver.
* "Sensor"-like Captcha Mode (BETA)
* Cloudflare Compatibility

## Contributing
Currently the Project is closed-source for the public.
If you would like to help us anyways, you can do so if you find Bypasses or Bugs in our System.

## License
zeroCDN is currently closed-source, but is licensed under the [GNU General Public License v3.](https://www.gnu.org/licenses/gpl-3.0.txt)
