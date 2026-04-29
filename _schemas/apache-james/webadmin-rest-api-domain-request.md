---
description: Request body for domain operations
layout: schema
name: DomainRequest
properties_list:
- description: Email domain name
  name: domain
  type: string
provider_name: Apache James
provider_slug: apache-james
schema_file: json-schema/webadmin-rest-api-domain-request-schema.json
slug: webadmin-rest-api-domain-request
source_filename: webadmin-rest-api-domain-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-domain-request-schema.json\",\n  \"title\": \"DomainRequest\",\n  \"description\": \"Request body for domain operations\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\",\n      \"description\": \"Email domain name\",\n      \"example\": \"example.com\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-james/refs/heads/main/json-schema/webadmin-rest-api-domain-request-schema.json
tags:
- Email
- IMAP
- Java
- JMAP
- Mail Server
- Open Source
- SMTP
title: DomainRequest
---
