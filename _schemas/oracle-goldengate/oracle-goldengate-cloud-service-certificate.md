---
description: ''
layout: schema
name: Certificate
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: deploymentId
  type: string
- description: ''
  name: subject
  type: string
- description: ''
  name: issuer
  type: string
- description: ''
  name: isSelfSigned
  type: boolean
- description: ''
  name: md5Hash
  type: string
- description: ''
  name: publicKey
  type: string
- description: ''
  name: publicKeyAlgorithm
  type: string
- description: ''
  name: timeValidFrom
  type: string
- description: ''
  name: timeValidTo
  type: string
- description: ''
  name: serial
  type: string
- description: ''
  name: lifecycleState
  type: string
- description: ''
  name: timeCreated
  type: string
provider_name: Oracle GoldenGate
provider_slug: oracle-goldengate
schema_file: json-schema/oracle-goldengate-cloud-service-certificate-schema.json
slug: oracle-goldengate-cloud-service-certificate
source_filename: oracle-goldengate-cloud-service-certificate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Certificate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"deploymentId\": {\n      \"type\": \"string\"\n    },\n    \"subject\": {\n      \"type\": \"string\"\n    },\n    \"issuer\": {\n      \"type\": \"string\"\n    },\n    \"isSelfSigned\": {\n      \"type\": \"boolean\"\n    },\n    \"md5Hash\": {\n      \"type\": \"string\"\n    },\n    \"publicKey\": {\n      \"type\": \"string\"\n    },\n    \"publicKeyAlgorithm\": {\n      \"type\": \"string\"\n    },\n    \"timeValidFrom\": {\n      \"type\": \"string\"\n    },\n    \"timeValidTo\": {\n      \"type\": \"string\"\n    },\n    \"serial\": {\n      \"type\": \"string\"\n    },\n    \"lifecycleState\": {\n      \"type\": \"string\"\n    },\n    \"timeCreated\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-goldengate/refs/heads/main/json-schema/oracle-goldengate-cloud-service-certificate-schema.json
tags:
- CDC
- Data Integration
- Data Synchronization
- Database
- Enterprise
- Real-Time Replication
title: Certificate
---
