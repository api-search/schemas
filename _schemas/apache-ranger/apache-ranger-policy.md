---
description: Ranger security policy definition
layout: schema
name: Policy
properties_list:
- description: Policy identifier
  name: id
  type: integer
- description: Policy name
  name: name
  type: string
- description: Service type this policy applies to (hdfs, hive, hbase)
  name: serviceType
  type: string
- description: Service name this policy applies to
  name: serviceName
  type: string
- description: Policy description
  name: description
  type: string
- description: Whether the policy is active
  name: isEnabled
  type: boolean
- description: Whether audit logging is enabled
  name: isAuditEnabled
  type: boolean
- description: Resources protected by this policy
  name: resources
  type: object
- description: ''
  name: policyItems
  type: array
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-policy-schema.json
slug: apache-ranger-policy
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: Policy
---
