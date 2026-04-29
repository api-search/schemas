---
description: ''
layout: schema
name: ScalingPolicy
properties_list:
- description: Policy name
  name: name
  type: string
- description: Target cluster
  name: clusterName
  type: string
- description: Whether the policy is active
  name: enabled
  type: boolean
- description: Minimum number of cluster members
  name: minMembers
  type: integer
- description: Maximum number of cluster members
  name: maxMembers
  type: integer
- description: ''
  name: scaleUpTrigger
  type: object
- description: ''
  name: scaleDownTrigger
  type: object
- description: Cooldown period in seconds between scaling events
  name: cooldownPeriod
  type: integer
provider_name: IBM WebSphere
provider_slug: websphere
schema_file: json-schema/websphere-liberty-collective-controller-rest-scaling-policy-schema.json
slug: websphere-liberty-collective-controller-rest-scaling-policy
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScalingPolicy\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Policy name\"\n    },\n    \"clusterName\": {\n      \"type\": \"string\",\n      \"description\": \"Target cluster\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the policy is active\"\n    },\n    \"minMembers\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum number of cluster members\"\n    },\n    \"maxMembers\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of cluster members\"\n    },\n    \"scaleUpTrigger\": {\n      \"type\": \"object\"\n    },\n    \"scaleDownTrigger\": {\n      \"type\": \"object\"\n    },\n    \"cooldownPeriod\": {\n      \"type\": \"integer\",\n      \"description\": \"Cooldown period in seconds between scaling events\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/websphere/refs/heads/main/json-schema/websphere-liberty-collective-controller-rest-scaling-policy-schema.json
tags:
- Application Server
- Cloud Native
- Enterprise Java
- J2EE
- Microservices
- Middleware
title: ScalingPolicy
---
