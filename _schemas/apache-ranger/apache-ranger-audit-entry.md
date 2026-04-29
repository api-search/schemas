---
description: Single access audit log entry
layout: schema
name: AuditEntry
properties_list:
- description: Audit entry identifier
  name: id
  type: string
- description: User who accessed the resource
  name: user
  type: string
- description: Type of resource accessed
  name: resourceType
  type: string
- description: Path of the accessed resource
  name: resourcePath
  type: string
- description: Type of access (read, write, etc.)
  name: accessType
  type: string
- description: Access result (1=allowed, 0=denied)
  name: result
  type: integer
- description: ACL enforcer that made the decision
  name: aclEnforcer
  type: string
- description: Agent/plugin that reported the audit
  name: agentId
  type: string
- description: Repository/service name
  name: repoName
  type: string
- description: Session identifier
  name: sessionId
  type: string
- description: Client IP address
  name: clientIP
  type: string
- description: Time of access event
  name: eventTime
  type: string
provider_name: Apache Ranger
provider_slug: apache-ranger
schema_file: json-schema/apache-ranger-audit-entry-schema.json
slug: apache-ranger-audit-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-audit-entry-schema.json\",\n  \"title\": \"AuditEntry\",\n  \"description\": \"Single access audit log entry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Audit entry identifier\"\n    },\n    \"user\": {\n      \"type\": \"string\",\n      \"description\": \"User who accessed the resource\"\n    },\n    \"resourceType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of resource accessed\"\n    },\n    \"resourcePath\": {\n      \"type\": \"string\",\n      \"description\": \"Path of the accessed resource\"\n    },\n    \"accessType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of access (read, write, etc.)\"\n    },\n    \"result\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Access result (1=allowed, 0=denied)\"\n    },\n    \"aclEnforcer\": {\n      \"type\": \"string\",\n      \"description\": \"ACL enforcer that made the decision\"\n    },\n    \"agentId\": {\n      \"type\": \"string\",\n      \"description\": \"Agent/plugin that reported the audit\"\n    },\n    \"repoName\": {\n      \"type\": \"string\",\n      \"description\": \"Repository/service name\"\n    },\n    \"sessionId\": {\n      \"type\": \"string\",\n      \"description\": \"Session identifier\"\n    },\n    \"clientIP\": {\n      \"type\": \"string\",\n      \"description\": \"Client IP address\"\n    },\n    \"eventTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time of access event\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ranger/refs/heads/main/json-schema/apache-ranger-audit-entry-schema.json
tags:
- Access Control
- Authorization
- Hadoop
- Policy Management
- Security
- Apache
- Open Source
title: AuditEntry
---
