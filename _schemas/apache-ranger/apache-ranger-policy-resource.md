---
description: Resource specification in a Ranger policy
layout: schema
name: PolicyResource
properties_list:
- description: Resource values (paths, tables, etc.)
  name: values
  type: array
- description: Whether to apply recursively
  name: isRecursive
  type: boolean
- description: Whether this is an exclusion list
  name: isExcludes
  type: boolean
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-policy-resource-schema.json
slug: apache-ranger-policy-resource
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: PolicyResource
---
