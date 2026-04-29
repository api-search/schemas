---
description: A VMware vCenter client registered with the Application Migration Service
layout: schema
name: VcenterClient
properties_list:
- description: vCenter client ID
  name: vcenterClientID
  type: string
- description: ARN of the vCenter client
  name: arn
  type: string
- description: vCenter server hostname
  name: hostname
  type: string
- description: vCenter UUID
  name: vcenterUUID
  type: string
- description: Datacenter name
  name: datacenterName
  type: string
- description: Date/time client was last seen
  name: lastSeenDatetime
  type: string
- description: Tags applied to source servers discovered by this client
  name: sourceServerTags
  type: object
- description: Tags on the vCenter client
  name: tags
  type: object
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-vcenter-client-schema.json
slug: application-migration-service-vcenter-client
source_filename: application-migration-service-vcenter-client-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-vcenter-client-schema.json\",\n  \"title\": \"VcenterClient\",\n  \"description\": \"A VMware vCenter client registered with the Application Migration Service\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vcenterClientID\": {\n      \"type\": \"string\",\n      \"description\": \"vCenter client ID\"\n    },\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the vCenter client\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"vCenter server hostname\"\n    },\n    \"vcenterUUID\": {\n      \"type\": \"string\",\n      \"description\": \"vCenter UUID\"\n    },\n    \"datacenterName\": {\n      \"type\": \"string\",\n      \"description\": \"Datacenter name\"\n    },\n    \"lastSeenDatetime\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Date/time client was last seen\"\n    },\n    \"sourceServerTags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags applied to source servers discovered by this client\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags on the vCenter client\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-vcenter-client-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: VcenterClient
---
