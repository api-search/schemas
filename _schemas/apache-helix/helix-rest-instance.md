---
description: Helix cluster instance (participant) configuration
layout: schema
name: Instance
properties_list:
- description: Instance name
  name: id
  type: string
- description: Hostname of the instance
  name: hostName
  type: string
- description: Port number
  name: port
  type: integer
- description: Whether the instance is enabled
  name: enabled
  type: boolean
- description: Instance tags
  name: tags
  type: array
provider_name: Apache Helix
provider_slug: apache-helix
schema_file: json-schema/helix-rest-instance-schema.json
slug: helix-rest-instance
tags:
- Apache
- Cluster Management
- Distributed Systems
- Open Source
- Partitioning
- Replication
title: Instance
---
