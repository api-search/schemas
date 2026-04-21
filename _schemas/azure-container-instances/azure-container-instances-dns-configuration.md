---
description: DNS configuration for the container group.
layout: schema
name: DnsConfiguration
properties_list:
- description: The DNS servers for the container group.
  name: nameServers
  type: array
- description: The DNS options for the container group.
  name: options
  type: string
- description: The DNS search domains for hostname lookup in the container group.
  name: searchDomains
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-dns-configuration-schema.json
slug: azure-container-instances-dns-configuration
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: DnsConfiguration
---
