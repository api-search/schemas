---
description: Describes a reserved node. You can call the <a>DescribeReservedNodeOfferings</a> API to obtain the available reserved node offerings.
layout: schema
name: ReservedNode
properties_list:
- description: ''
  name: ReservedNodeId
  type: object
- description: ''
  name: ReservedNodeOfferingId
  type: object
- description: ''
  name: NodeType
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: Duration
  type: object
- description: ''
  name: FixedPrice
  type: object
- description: ''
  name: UsagePrice
  type: object
- description: ''
  name: CurrencyCode
  type: object
- description: ''
  name: NodeCount
  type: object
- description: ''
  name: State
  type: object
- description: ''
  name: OfferingType
  type: object
- description: ''
  name: RecurringCharges
  type: object
- description: ''
  name: ReservedNodeOfferingType
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-reserved-node-schema.json
slug: redshift-reserved-node
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReservedNodeId\": {},\n    \"ReservedNodeOfferingId\": {},\n    \"NodeType\": {},\n    \"StartTime\": {},\n    \"Duration\": {},\n    \"FixedPrice\": {},\n    \"UsagePrice\": {},\n    \"CurrencyCode\": {},\n    \"NodeCount\": {},\n    \"State\": {},\n    \"OfferingType\": {},\n    \"RecurringCharges\": {},\n    \"ReservedNodeOfferingType\": {}\n  },\n  \"description\": \"Describes a reserved node. You can call the <a>DescribeReservedNodeOfferings</a> API to obtain the available reserved node offerings. \",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-reserved-node-schema.json\",\n  \"title\": \"ReservedNode\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-reserved-node-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ReservedNode
---
