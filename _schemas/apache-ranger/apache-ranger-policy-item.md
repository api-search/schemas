---
description: Policy item defining access permissions
layout: schema
name: PolicyItem
properties_list:
- description: Users granted access
  name: users
  type: array
- description: Groups granted access
  name: groups
  type: array
- description: ''
  name: accesses
  type: array
- description: ''
  name: conditions
  type: array
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-policy-item-schema.json
slug: apache-ranger-policy-item
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: PolicyItem
---
