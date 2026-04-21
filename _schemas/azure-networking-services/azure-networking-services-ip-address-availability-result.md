---
description: Response for CheckIPAddressAvailability API service call.
layout: schema
name: IPAddressAvailabilityResult
properties_list:
- description: Private IP address availability.
  name: available
  type: boolean
- description: Contains other available private IP addresses if the asked for address is taken.
  name: availableIPAddresses
  type: array
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-ip-address-availability-result-schema.json
slug: azure-networking-services-ip-address-availability-result
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: IPAddressAvailabilityResult
---
