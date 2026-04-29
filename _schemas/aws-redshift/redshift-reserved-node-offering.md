---
description: Describes a reserved node offering.
layout: schema
name: ReservedNodeOffering
properties_list:
- description: ''
  name: ReservedNodeOfferingId
  type: object
- description: ''
  name: NodeType
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
schema_file: json-schema/redshift-reserved-node-offering-schema.json
slug: redshift-reserved-node-offering
source_filename: redshift-reserved-node-offering-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReservedNodeOfferingId\": {},\n    \"NodeType\": {},\n    \"Duration\": {},\n    \"FixedPrice\": {},\n    \"UsagePrice\": {},\n    \"CurrencyCode\": {},\n    \"OfferingType\": {},\n    \"RecurringCharges\": {},\n    \"ReservedNodeOfferingType\": {}\n  },\n  \"description\": \"Describes a reserved node offering.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-reserved-node-offering-schema.json\",\n  \"title\": \"ReservedNodeOffering\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-reserved-node-offering-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: ReservedNodeOffering
---
