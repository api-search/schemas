---
description: Discovered properties of the source server
layout: schema
name: SourceProperties
properties_list:
- description: Date/time properties were last updated
  name: lastUpdatedDateTime
  type: string
- description: AWS instance type recommended for this server
  name: recommendedInstanceType
  type: string
- description: identificationHints
  name: identificationHints
  type: string
- description: Network interfaces on the source server
  name: networkInterfaces
  type: array
- description: Disks on the source server
  name: disks
  type: array
- description: CPUs on the source server
  name: cpus
  type: array
- description: RAM in bytes
  name: ramBytes
  type: integer
- description: os
  name: os
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-source-properties-schema.json
slug: application-migration-service-source-properties
source_filename: application-migration-service-source-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-source-properties-schema.json\",\n  \"title\": \"SourceProperties\",\n  \"description\": \"Discovered properties of the source server\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lastUpdatedDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time properties were last updated\"\n    },\n    \"recommendedInstanceType\": {\n      \"type\": \"string\",\n      \"description\": \"AWS instance type recommended for this server\"\n    },\n    \"identificationHints\": {\n      \"type\": \"string\",\n      \"description\": \"identificationHints\"\n    },\n    \"networkInterfaces\": {\n      \"type\": \"array\",\n      \"description\": \"Network interfaces on the source server\"\n    },\n    \"disks\": {\n      \"type\": \"array\",\n      \"description\": \"Disks\
  \ on the source server\"\n    },\n    \"cpus\": {\n      \"type\": \"array\",\n      \"description\": \"CPUs on the source server\"\n    },\n    \"ramBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"RAM in bytes\"\n    },\n    \"os\": {\n      \"type\": \"string\",\n      \"description\": \"os\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-source-properties-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: SourceProperties
---
