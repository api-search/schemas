---
description: Hints used to identify the source server
layout: schema
name: IdentificationHints
properties_list:
- description: Fully qualified domain name
  name: fqdn
  type: string
- description: Hostname
  name: hostname
  type: string
- description: VMware UUID
  name: vmWareUuid
  type: string
- description: AWS instance ID if previously in AWS
  name: awsInstanceID
  type: string
- description: VMware path
  name: vmPath
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-identification-hints-schema.json
slug: application-migration-service-identification-hints
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-identification-hints-schema.json\",\n  \"title\": \"IdentificationHints\",\n  \"description\": \"Hints used to identify the source server\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"fqdn\": {\n      \"type\": \"string\",\n      \"description\": \"Fully qualified domain name\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname\"\n    },\n    \"vmWareUuid\": {\n      \"type\": \"string\",\n      \"description\": \"VMware UUID\"\n    },\n    \"awsInstanceID\": {\n      \"type\": \"string\",\n      \"description\": \"AWS instance ID if previously in AWS\"\n    },\n    \"vmPath\": {\n      \"type\": \"string\",\n      \"description\": \"VMware path\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-identification-hints-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: IdentificationHints
---
