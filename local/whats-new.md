---

copyright:
  years: 2015, 2020
lastupdated: "2020-12-24"

keywords: new features, updates, not supported

subcollection: Cloudant

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}
{:tip: .tip}
{:note: .note}
{:important: .important}
{:deprecated: .deprecated}
{:external: target="_blank" .external}

<!-- Acrolinx: 2017-05-10 -->

# What's new
{: #whats-new-cloudant-local}

Read about the new features in {{site.data.keyword.IBM}} Cloudant&reg; Data Layer Local Edition ({{site.data.keyword.cloudant_local_notm}})
version 1.1.0.
{: shortdesc}

## Eliminate plain text passwords
{: #eliminate-plain-text-passwords}

Since intercepting plain text passwords and gaining access to your system is simple, you can no longer use plain text passwords with {{site.data.keyword.cloudant_local_notm}}. 

## Self-extracting archive installer
{: #self-extracting-archive-installer}

When you use the self-extracting archive, it is no longer necessary to unpack archive files. 

## Python wheels
{: #python-wheels}

Python wheels reduce, or even eliminate, the need for you to download Python dependencies and can decrease incompatibilities. 

## CouchDB 2.0 compatible
{: #couchdb-2.0-compatible}

{{site.data.keyword.cloudant_local_notm}} is now compatible with CouchDB 2.0. 

## Python virtual environments
{: #python-virtual-environments}

Each Python application now runs within its own virtual
environment, eliminating version incompatibility between each application's Python modules.

## Database logs
{: #database-logging}

Simplified the following database logs issues.

Database logs no longer requires a separate configuration file, but can be configured by using `.ini` files. 

By default, the database uses syslog to log to `/var/log/cloudant/cloudant.log`, but you can direct it to other hosts by setting `syslog_host` = `your_host` in the `[log]` section of the `local.ini`.

Additionally, the `cloudant.log`, `clouseau.log`, and `metrics.log` files, 
which are located in `/var/log/cloudant/`, are automatically rotated to use the configuration at `/etc/logrotate.d/cloudant`.

## Multiple bug fixes 
{: #multiple-bug-fixes}

Implemented multiple bug fixes to improve performance
and correct other issues. 

## Rolling upgrade not supported
{: #rolling-upgrade-not-supported}
  
{{site.data.keyword.cloudant_local_notm}} does not support rolling upgrades.