---
description: Ranger user definition
layout: schema
name: RangerUser
properties_list:
- description: User identifier
  name: id
  type: integer
- description: Username
  name: name
  type: string
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: emailAddress
  type: string
- description: User source (0=internal, 1=LDAP/AD)
  name: userSource
  type: integer
- description: User status (1=active, 0=disabled)
  name: status
  type: integer
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-ranger-user-schema.json
slug: apache-ranger-ranger-user
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: RangerUser
---
