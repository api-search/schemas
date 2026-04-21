---
description: Ranger user group
layout: schema
name: RangerGroup
properties_list:
- description: Group identifier
  name: id
  type: integer
- description: Group name
  name: name
  type: string
- description: Group description
  name: description
  type: string
- description: Group source (0=internal, 1=LDAP/AD)
  name: groupSource
  type: integer
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-ranger-group-schema.json
slug: apache-ranger-ranger-group
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: RangerGroup
---
