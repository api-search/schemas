---
description: An aggregate (local tier) is a collection of physical disks that provides a pool of storage from which FlexVol volumes are provisioned.
layout: schema
name: Aggregate
properties_list:
- description: Aggregate UUID
  name: uuid
  type: string
- description: Aggregate name
  name: name
  type: string
- description: Aggregate operational state
  name: state
  type: string
- description: Aggregate space usage
  name: space
  type: object
- description: Block storage configuration
  name: block_storage
  type: object
- description: Aggregate encryption configuration
  name: data_encryption
  type: object
- description: FabricPool configuration
  name: cloud_storage
  type: object
- description: Time when the aggregate was created
  name: create_time
  type: string
provider_name: NetApp
provider_slug: netapp
schema_file: json-schema/netapp-ontap-aggregate-schema.json
slug: netapp-ontap-aggregate
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Aggregate\",\n  \"type\": \"object\",\n  \"description\": \"An aggregate (local tier) is a collection of physical disks that provides a pool of storage from which FlexVol volumes are provisioned.\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Aggregate UUID\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Aggregate name\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Aggregate operational state\"\n    },\n    \"space\": {\n      \"type\": \"object\",\n      \"description\": \"Aggregate space usage\"\n    },\n    \"block_storage\": {\n      \"type\": \"object\",\n      \"description\": \"Block storage configuration\"\n    },\n    \"data_encryption\": {\n      \"type\": \"object\",\n      \"description\": \"Aggregate encryption configuration\"\n    },\n    \"cloud_storage\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"FabricPool configuration\"\n    },\n    \"create_time\": {\n      \"type\": \"string\",\n      \"description\": \"Time when the aggregate was created\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/netapp/refs/heads/main/json-schema/netapp-ontap-aggregate-schema.json
tags:
- Cloud
- Data Management
- Hybrid Cloud
- Infrastructure
- Storage
title: Aggregate
---
