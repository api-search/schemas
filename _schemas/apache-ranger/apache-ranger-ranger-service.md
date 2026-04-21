---
description: Ranger service definition
layout: schema
name: RangerService
properties_list:
- description: Service identifier
  name: id
  type: integer
- description: Service name
  name: name
  type: string
- description: Service type (hdfs, hive, hbase, kafka, etc.)
  name: type
  type: string
- description: Service description
  name: description
  type: string
- description: Whether the service is active
  name: isEnabled
  type: boolean
- description: Service connection configuration
  name: configs
  type: object
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-ranger-service-schema.json
slug: apache-ranger-ranger-service
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: RangerService
---
