﻿# Installing Amplia on Ubuntu Server

<!-- https://docs.microsoft.com/en-us/aspnet/core/host-and-deploy/linux-nginx?view=aspnetcore-2.2 -->

Before you start, make sure you have read the section [Planning before installation](../index.md#planning).

[!include[Database operation mode](../includes/database-mode.md)]

## Prerequisites

* Ubuntu x64 version 16.04, 18.04 or 19.04

[!include[Common prerequisites](../includes/common-requisites.md)]

[!include[Install ASP.NET Core Runtime 2.2](../../../includes/linux/ubuntu/install-aspnetcore-22.md)]

## Install Amplia

[!include[Common Linux installation](includes/common-linux-install.md)]

## Set up a reverse proxy server

[!include[Install Nginx](../../../includes/linux/ubuntu/install-nginx.md)]

Create a site configuration file for Amplia:

[!include[Create site](../../../../../includes/amplia/ubuntu/create-site.md)]

[!include[Configure site](includes/configure-site.md)]

Enable the site:

[!include[Enable site](../../../../../includes/amplia/ubuntu/enable-site.md)]

[!include[Reload nginx and test site](includes/reload-and-test.md)]

## See also

* [Updating Amplia on Linux](update.md)
* [Troubleshooting](troubleshoot/index.md)
