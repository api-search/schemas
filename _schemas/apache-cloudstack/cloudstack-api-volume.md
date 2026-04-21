---
description: A CloudStack storage volume attached to a virtual machine.
layout: schema
name: Volume
properties_list:
- description: UUID of the volume.
  name: id
  type: string
- description: Display name of the volume.
  name: name
  type: string
- description: Volume type (ROOT or DATADISK).
  name: type
  type: string
- description: Current state of the volume.
  name: state
  type: string
- description: Volume size in bytes.
  name: size
  type: integer
- description: UUID of the virtual machine this volume is attached to.
  name: virtualmachineid
  type: string
provider_name: Apache CloudStack
provider_slug: apache-cloudstack
schema_file: json-schema/cloudstack-api-volume-schema.json
slug: cloudstack-api-volume
tags:
- Apache
- Cloud
- IaaS
- Infrastructure
- Open Source
- Virtualization
title: Volume
---
