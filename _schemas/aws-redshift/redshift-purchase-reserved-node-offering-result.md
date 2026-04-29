---
description: PurchaseReservedNodeOfferingResult schema from Amazon Redshift
layout: schema
name: PurchaseReservedNodeOfferingResult
properties_list:
- description: Describes a reserved node. You can call the <a>DescribeReservedNodeOfferings</a> API to obtain the available reserved node offerings.
  name: ReservedNode
  type: object
provider_name: AWS Redshift
provider_slug: aws-redshift
schema_file: json-schema/redshift-purchase-reserved-node-offering-result-schema.json
slug: redshift-purchase-reserved-node-offering-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"ReservedNode\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"ReservedNodeId\": {},\n        \"ReservedNodeOfferingId\": {},\n        \"NodeType\": {},\n        \"StartTime\": {},\n        \"Duration\": {},\n        \"FixedPrice\": {},\n        \"UsagePrice\": {},\n        \"CurrencyCode\": {},\n        \"NodeCount\": {},\n        \"State\": {},\n        \"OfferingType\": {},\n        \"RecurringCharges\": {},\n        \"ReservedNodeOfferingType\": {}\n      },\n      \"description\": \"Describes a reserved node. You can call the <a>DescribeReservedNodeOfferings</a> API to obtain the available reserved node offerings. \"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-purchase-reserved-node-offering-result-schema.json\",\n  \"title\": \"PurchaseReservedNodeOfferingResult\"\
  ,\n  \"description\": \"PurchaseReservedNodeOfferingResult schema from Amazon Redshift\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-redshift/refs/heads/main/json-schema/redshift-purchase-reserved-node-offering-result-schema.json
tags:
- Analytics
- Big Data
- Cloud Database
- Data Warehouse
- SQL
title: PurchaseReservedNodeOfferingResult
---
