﻿# Installing Amplia on Oracle Linux

<!-- https://docs.microsoft.com/en-us/aspnet/core/host-and-deploy/linux-nginx?view=aspnetcore-2.2 -->

Before you start, make sure you have read the section [Planning before installation](../index.md#planning).

[!include[Database operation mode](../includes/database-mode.md)]

## Prerequisites

* Oracle Linux 7.x

[!include[Common prerequisites](../includes/common-requisites.md)]

[!include[Install ASP.NET Core Runtime](../../../includes/linux/oracle/install-aspnetcore-22.md)]

## Install Amplia

> [!NOTE]
> Some steps use the `nano` command, which might not be installed on your system. Feel free to replace the command by `vi` or install nano with `yum install nano`

[!include[Common Linux installation](includes/common-linux-install.md)]

## Set up a reverse proxy server

[!include[Install Nginx](../../../includes/linux/oracle/install-nginx.md)]

Create a site configuration file for Amplia:

[!include[Create site](../../../../../includes/amplia/centos/create-site.md)]

[!include[Configure site](includes/configure-site.md)]

Allow Nginx to access the Amplia service:

[!include[Allow service access](../../../../../includes/linux/centos/allow-service-access.md)]

[!include[Reload nginx and test site](includes/reload-and-test.md)]

Allow HTTP and HTTPS traffic to your system (if not already allowed):

[!include[Allow traffic](../../../../../includes/linux/centos/allow-http.md)]

## See also

* [Updating Amplia on Linux](update.md)
* [Troubleshooting](troubleshoot/index.md)
