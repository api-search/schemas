---
description: Resource schema from AT&T API
layout: schema
name: Resource
properties_list:
- description: Unique resource identifier
  name: id
  type: string
- description: Device or SIM name
  name: name
  type: string
- description: Type of resource
  name: resourceType
  type: string
- description: Resource operational status
  name: status
  type: string
- description: Device IMEI or SIM ICCID
  name: serialNumber
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/mvnx-api-resource-schema.json
slug: mvnx-api-resource
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: Resource
---
