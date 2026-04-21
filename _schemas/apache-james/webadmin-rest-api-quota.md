---
description: Storage and message quota configuration
layout: schema
name: Quota
properties_list:
- description: Maximum number of messages (null for unlimited)
  name: count
  type: integer
- description: Maximum storage size in bytes (null for unlimited)
  name: size
  type: integer
provider_name: Apache James
provider_slug: apache-james
schema_file: json-schema/webadmin-rest-api-quota-schema.json
slug: webadmin-rest-api-quota
tags:
- Email
- IMAP
- Java
- JMAP
- Mail Server
- Open Source
- SMTP
title: Quota
---
