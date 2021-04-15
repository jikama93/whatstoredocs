# How to enable PHP zip extension in cPanel

_Are you looking to enable PHP zip extension in cPanel?_ We can help you.

PHP websites using zip files needs zip extensions for data processing.

At Bobcares, we receive requests to enable PHP zip extensions as a part of our [Server Management Services](https://bobcares.com/server-management-services/).

Today, let’s see how our [Support Engineers](https://bobcares.com/server-management-services/) enable PHP zip extension in cPanel.

## Why do we need the PHP zip extension?

Website owners always look for ways to optimize website files. Zipping is one way to reduce file size.

A zip archive file format supports lossless data compression, thereby making it suitable for sending and storing data.

If websites use a zip file format, it needs a zip extension to process it. That is, zip extension allows the users to read and write into the zip files.

Now, let’s see how our [Support Engineers](https://bobcares.com/server-management-services/) enable PHP zip extensions in cPanel.

## How to enable the PHP zip extension in cPanel?

1. Firstly, we log into cPanel and click on the **PHP PEAR Packages** available under the **SOFTWARE** section. The icon appears as in the image.

![Enable PHP zip extension cPanel](data:image/svg+xml,%3Csvg%20xmlns=%22http://www.w3.org/2000/svg%22%20viewBox=%220%200%201273%20405%22%3E%3C/svg%3E)

2. Then we type zip in the search bar, and **Archive\_Zip** will be available. Here, we click on the install icon.

3. After installing Archive\_Zip, we go to the previous step and click the **Select PHP Version** icon.

4. Now, the Archive\_Zip is visible here. Click the checkbox of the zip extension. And hit the save button to add the Archive\_Zip to the current PHP version. This would install the PHP Zip extension.

## How to enable PHP zip extension in WHM?

Zip extension is a very basic requirement for websites nowadays. So we enable it in all the servers we manage. Let’s see how we enable it via WHM.

Initially, we login to WHM and navigate as follows,

**Software** &gt;&gt; **EasyApache 4** &gt;&gt; **Customize** &gt;&gt; **PHP extensions**. Here we search for zip and enable _phpx.x-php-zip_ for all versions. Finally, we click on **Review** and **Provision**.

This enables the zip extension for all the PHP websites in the server.

## Common errors while enabling PHP Zip extension

Now, let’s see a few common errors our customers reported to us while enabling the PHP zip extension.

### 1. Missing library

Recently, one of our customers approached us with the below error message

```text
PHP ZipArchive Library is missing or disabled
```

Our [Support Engineers](https://bobcares.com/server-management-services/) checked the current PHP version using the command,

```text
php -v
```

He used CentOS 6 with Apache and PHP 7.0. The PHP 7 provides a _php7.0-zip_ package. We installed it using the command,

```text
yum install php7.0-zip
```

We used the below command to check the libraries,

```text
yum list installed | grep -i php
```

Lastly, we ran the below command to restart Apache,

```text
service httpd restart
```

Finally, this fixed the error.

### 2. Installation command error

The PHP zip extensions can be enabled through commands as well. So, few customers try to install it via commands itself. But mistakes in the command lead to errors.

Here is an example where the customer experienced an error due to incorrect command.

The customer received the error `Class ZipExtension not found`. He was using CentOS 7 and PHP 7.0.27.

Our [Support Engineers](https://bobcares.com/server-management-services/) checked the command he used. The command was,

```text
yum install php70-php-pecl-zip
```

The actual package was _php-pecl-zip.x86\_64_. So we installed it using the command,

```text
yum install php70-php-pecl-zip.x86_64
```

And then, we enabled it by running the command,

```text
echo "extension=zip.so" >> /etc/php.d/zip.ini
```

This fixed the error and the PHP extension was enabled.

**\[Need assistance in enabling the PHP extension? –** [**We’ll help you**](https://bobcares.com/server-management-services/)**.\]**

## Conclusion

In short, PHP websites using zip files require zip extensions for data processing. Today, we saw how our [Support Engineers](https://bobcares.com/server-management-services/) enabled PHP zip extension in cPanel.

## PREVENT YOUR SERVER FROM CRASHING!

Never again lose customers to poor server speed! Let us help you.

Our server experts will monitor & maintain your server 24/7 so that it remains lightning fast and secure.

[GET STARTED](https://bobcares.com/server-management-services/)

 var google\_conversion\_label = "owonCMyG5nEQ0aD71QM";

