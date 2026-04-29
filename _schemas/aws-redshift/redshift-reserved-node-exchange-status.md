---
description: Reserved-node status details, such as the source reserved-node identifier, the target reserved-node identifier, the node type, the node count, and other details.
layout: schema
name: ReservedNodeExchangeStatus
properties_list:
- description: ''
  name: ReservedNodeExchangeRequestId
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: RequestTime
  type: object
- description: ''
  name: SourceReservedNodeId
  type: object
- description: ''
  name: SourceReservedNodeType
  type: object
- description: ''
  name: SourceReservedNodeCount
  type: object
- description: ''
  name: TargetReservedNodeOfferingId
  type: object
- description: ''
  name: TargetReservedNodeType
  type: object
- description: ''
  name: TargetReservedNodeCount
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-reserved-node-exchange-status-schema.json
slug: redshift-reserved-node-exchange-status
source_filename: redshift-reserved-node-exchange-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReservedNodeExchangeRequestId\": {},\n    \"Status\": {},\n    \"RequestTime\": {},\n    \"SourceReservedNodeId\": {},\n    \"SourceReservedNodeType\": {},\n    \"SourceReservedNodeCount\": {},\n    \"TargetReservedNodeOfferingId\": {},\n    \"TargetReservedNodeType\": {},\n    \"TargetReservedNodeCount\": {}\n  },\n  \"description\": \"Reserved-node status details, such as the source reserved-node identifier, the target reserved-node identifier, the node type, the node count, and other details.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-reserved-node-exchange-status-schema.json\",\n  \"title\": \"ReservedNodeExchangeStatus\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-reserved-node-exchange-status-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ReservedNodeExchangeStatus
---
