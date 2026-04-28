---
description: Schema for a device registration on Cisco Expressway. Represents an endpoint or device currently registered with the Expressway using SIP or H.323 protocols, including contact address, registration time, and subzone assignment.
layout: schema
name: Cisco Expressway Registration
properties_list:
- description: Registered alias of the device, such as a SIP URI or H.323 alias
  name: Alias
  type: string
- description: Registration protocol type
  name: Type
  type: string
- description: Network contact address of the device, including IP address and port
  name: ContactAddress
  type: string
- description: ISO 8601 timestamp when the device registered
  name: RegisteredAt
  type: string
- description: ISO 8601 timestamp when the registration expires and must be renewed
  name: ExpiresAt
  type: string
- description: Type or model of the registered device as reported during registration
  name: DeviceType
  type: string
- description: Subzone where the device is registered based on IP address ranges or alias patterns. Endpoints not matching any configured subzone are assigned to the DefaultSubzone.
  name: Subzone
  type: string
provider_name: Cisco Expressway
provider_slug: cisco-expressway
schema_file: json-schema/cisco-expressway-registration-schema.json
slug: cisco-expressway-registration
tags:
- Collaboration
- Firewall Traversal
- H.323
- Session Border Controller
- SIP
- Unified Communications
- Video Conferencing
title: Cisco Expressway Registration
---
