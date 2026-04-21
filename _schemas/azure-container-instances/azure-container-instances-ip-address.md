---
description: IP address for the container group.
layout: schema
name: IpAddress
properties_list:
- description: The Dns name label for the IP.
  name: dnsNameLabel
  type: string
- description: The FQDN for the IP.
  name: fqdn
  type: string
- description: The IP exposed to the public internet.
  name: ip
  type: string
- description: The list of ports exposed on the container group.
  name: ports
  type: array
- description: Specifies if the IP is exposed to the public internet or private VNET.
  name: type
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-ip-address-schema.json
slug: azure-container-instances-ip-address
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: IpAddress
---
