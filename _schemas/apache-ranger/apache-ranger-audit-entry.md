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
