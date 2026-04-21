---
description: Health check result for a single component
layout: schema
name: ComponentCheck
properties_list:
- description: Component name
  name: componentName
  type: string
- description: URL-encoded component name
  name: escapedComponentName
  type: string
- description: Component health status
  name: status
  type: string
- description: Reason for unhealthy status (if applicable)
  name: cause
  type: string
provider_name: Apache James
provider_slug: apache-james
schema_file: json-schema/webadmin-rest-api-component-check-schema.json
slug: webadmin-rest-api-component-check
tags:
- Email
- IMAP
- Java
- JMAP
- Mail Server
- Open Source
- SMTP
title: ComponentCheck
---
