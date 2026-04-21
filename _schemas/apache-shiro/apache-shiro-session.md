---
description: Shiro session information
layout: schema
name: Session
properties_list:
- description: Session identifier
  name: id
  type: string
- description: Session creation time
  name: startTimestamp
  type: string
- description: Last access time
  name: lastAccessTime
  type: string
- description: Session timeout in milliseconds
  name: timeout
  type: integer
- description: Host of the session initiator
  name: host
  type: string
- description: Whether the session has expired
  name: expired
  type: boolean
provider_name: Apache Shiro
provider_slug: apache-shiro
schema_file: json-schema/apache-shiro-session-schema.json
slug: apache-shiro-session
tags:
- Authentication
- Authorization
- Cryptography
- Java
- Security
- Apache
- Open Source
title: Session
---
