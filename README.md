# azure-sophos-xg
Deployment template to deploy Sophos XG firewall to Azure.

Mirrored source (https://github.com/sophos-iaas/xg-azure/) and confirmed working. Will make later versions not create an unused availbility set and also set static private IPs on NICs.

Deploying
=========

1.) Open template link: https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FNorm-Reeves%2Fazure-sophos-xg%2F1.0%2FmainTemplate.json

2.) Upload (and modify if needed) parameters.json. Take a look on the example values for template parameters in `mainTemplateParameters.json`.

Please note:
* The `adminPassword` has to be minimum 8 characters, **containing at least a lowercase letter, an uppercase letter, a number, and a special character.**

3) Deployment will start.
4) Wait until the deployment goes to state "Succeeded".

Connect to the VM instance
==========================
[https://full-dns-name:4444](https://full-dns-name:4444)


Reference for Full Setup
============
https://community.sophos.com/sophos-xg-firewall/f/recommended-reads/124683/sophos-firewall-reference-architecture-on-azure-with-dual-nic


Change Log:
============
1.0:
  • Mirrored source (https://github.com/sophos-iaas/xg-azure/) and confirmed working.
