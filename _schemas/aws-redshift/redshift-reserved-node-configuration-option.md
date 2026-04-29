---
description: Details for a reserved-node exchange. Examples include the node type for a reserved node, the price for a node, the node's state, and other details.
layout: schema
name: ReservedNodeConfigurationOption
properties_list:
- description: Describes a reserved node. You can call the <a>DescribeReservedNodeOfferings</a> API to obtain the available reserved node offerings.
  name: SourceReservedNode
  type: object
- description: ''
  name: TargetReservedNodeCount
  type: object
- description: Describes a reserved node offering.
  name: TargetReservedNodeOffering
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-reserved-node-configuration-option-schema.json
slug: redshift-reserved-node-configuration-option
source_filename: redshift-reserved-node-configuration-option-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"SourceReservedNode\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ReservedNodeId\": {},\n        \"ReservedNodeOfferingId\": {},\n        \"NodeType\": {},\n        \"StartTime\": {},\n        \"Duration\": {},\n        \"FixedPrice\": {},\n        \"UsagePrice\": {},\n        \"CurrencyCode\": {},\n        \"NodeCount\": {},\n        \"State\": {},\n        \"OfferingType\": {},\n        \"RecurringCharges\": {},\n        \"ReservedNodeOfferingType\": {}\n      },\n      \"description\": \"Describes a reserved node. You can call the <a>DescribeReservedNodeOfferings</a> API to obtain the available reserved node offerings. \"\n    },\n    \"TargetReservedNodeCount\": {},\n    \"TargetReservedNodeOffering\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ReservedNodeOfferingId\": {},\n        \"NodeType\": {},\n        \"Duration\": {},\n        \"FixedPrice\": {},\n        \"UsagePrice\"\
  : {},\n        \"CurrencyCode\": {},\n        \"OfferingType\": {},\n        \"RecurringCharges\": {},\n        \"ReservedNodeOfferingType\": {}\n      },\n      \"description\": \"Describes a reserved node offering.\"\n    }\n  },\n  \"description\": \"Details for a reserved-node exchange. Examples include the node type for a reserved node, the price for a node, the node's state, and other details.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-reserved-node-configuration-option-schema.json\",\n  \"title\": \"ReservedNodeConfigurationOption\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-reserved-node-configuration-option-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ReservedNodeConfigurationOption
---
