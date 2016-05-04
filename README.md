# PowerShell Empire Web


PowerShell Empire Web utilizes the [Empire REST API Server](https://github.com/PowerShellEmpire/Empire/wiki/RESTful-API). It is a web interface for using [PowerShell Empire](https://github.com/PowerShellEmpire/Empire/).


# Run Empire REST API Server


Get PowerShell Empire: https://github.com/PowerShellEmpire/Empire


./empire --headless --restport port --username empire_username --password empire_password


# Requirements


PHP Curl should be installed to use Empire Web.


## Install PHP Curl

```
sudo apt-get install php5-curl
```


## To check for PHP Curl

Command Line:
```
root@kali:~# php -i | grep -i curl
/etc/php5/cli/conf.d/20-curl.ini,
curl
cURL support => enabled
cURL Information => 7.47.0
```

PHP Script:
```
<?php
echo (function_exists('curl_version') ? "Curl found": "Curl not found");
?>
```


# Important


CSRF protection has not been implemented because it was affecting the working of Empire Web. It will be implemented in the next release.


Stay Calm. Stay Secure. Contribute :)


# Screenshots


![powershell-empire-web-login](https://cloud.githubusercontent.com/assets/5358495/14923483/160144b2-0e5b-11e6-95af-9dfbddd8c126.PNG)


![powershell-empire-web-about](https://cloud.githubusercontent.com/assets/5358495/14923495/244ab382-0e5b-11e6-8041-205ba35d7ac8.PNG)


![powershell-empire-web-dashboard](https://cloud.githubusercontent.com/assets/5358495/14923500/298853d6-0e5b-11e6-946e-cdf75e50c366.PNG)

