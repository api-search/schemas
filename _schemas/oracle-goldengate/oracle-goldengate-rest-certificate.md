---
description: ''
layout: schema
name: Certificate
properties_list:
- description: ''
  name: alias
  type: string
- description: ''
  name: subject
  type: string
- description: ''
  name: issuer
  type: string
- description: ''
  name: serialNumber
  type: string
- description: ''
  name: notBefore
  type: string
- description: ''
  name: notAfter
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-rest-certificate-schema.json
slug: oracle-goldengate-rest-certificate
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Certificate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alias\": {\n      \"type\": \"string\"\n    },\n    \"subject\": {\n      \"type\": \"string\"\n    },\n    \"issuer\": {\n      \"type\": \"string\"\n    },\n    \"serialNumber\": {\n      \"type\": \"string\"\n    },\n    \"notBefore\": {\n      \"type\": \"string\"\n    },\n    \"notAfter\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-rest-certificate-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Certificate
---
