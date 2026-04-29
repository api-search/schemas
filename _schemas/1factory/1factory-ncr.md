---
description: Ncr schema from 1Factory API
layout: schema
name: Ncr
properties_list: []
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-ncr-schema.json
slug: 1factory-ncr
source_filename: 1factory-ncr-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-ncr-schema.json\",\n  \"title\": \"Ncr\",\n  \"description\": \"Ncr schema from 1Factory API\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/Issue\"\n    },\n    {\n      \"properties\": {\n        \"description\": {\n          \"type\": \"string\",\n          \"nullable\": true,\n          \"maxLength\": 255,\n          \"description\": \"Description of the part.\",\n          \"example\": \"Three Lobe Shaft\"\n        },\n        \"use_as_is_quantity\": {\n          \"type\": \"number\",\n          \"nullable\": true,\n          \"description\": \"The number of parts that failed inspection that can be used as-is without rework or scrapping.\",\n          \"example\": 3\n        },\n        \"scrap_quantity\": {\n          \"type\": \"number\",\n          \"\
  nullable\": true,\n          \"description\": \"The number of parts that failed inspection that must be scrapped.\",\n          \"example\": 3\n        },\n        \"return_quantity\": {\n          \"type\": \"number\",\n          \"nullable\": true,\n          \"description\": \"The number of parts that failed inspection that must be returned to the supplier.\",\n          \"example\": 3\n        },\n        \"rework_quantity\": {\n          \"type\": \"number\",\n          \"nullable\": true,\n          \"description\": \"The number of parts that failed inspection that can be reworked to pass inspection.\",\n          \"example\": 3\n        },\n        \"repair_quantity\": {\n          \"type\": \"number\",\n          \"nullable\": true,\n          \"description\": \"The number of parts that failed inspection that can be repaired to pass inspection.\",\n          \"example\": 3\n        },\n        \"no_defect_quantity\": {\n          \"type\": \"number\",\n          \"nullable\": true,\n\
  \          \"description\": \"The number of parts in the lot that do not have any defects.\",\n          \"example\": 3\n        },\n        \"inventory_location\": {\n          \"type\": \"string\",\n          \"nullable\": true,\n          \"description\": \"\",\n          \"example\": \"Warehouse\"\n        },\n        \"rma_number\": {\n          \"type\": \"string\",\n          \"nullable\": true,\n          \"description\": \"RMA number, if any, for the returned parts in the NCR.\",\n          \"example\": \"rma-202405\"\n        },\n        \"rework_po\": {\n          \"type\": \"string\",\n          \"nullable\": true,\n          \"description\": \"\",\n          \"example\": \"po-202407-1\"\n        },\n        \"shipment\": {\n          \"type\": \"string\",\n          \"nullable\": true,\n          \"description\": \"Shipment number, if any, for parts in the NCR\",\n          \"example\": \"\"\n        },\n        \"mrb_meeting_notes\": {\n          \"type\": \"string\",\n \
  \         \"nullable\": true,\n          \"description\": \"Any meeting notes for this NCR from a MBR meeting.\",\n          \"example\": \"\"\n        },\n        \"mrb_dispositions\": {\n          \"type\": \"array\",\n          \"nullable\": false,\n          \"description\": \"MRB dispositions for this NCR.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"nullable\": false,\n                \"example\": \"REWORK\"\n              },\n              \"qty\": {\n                \"type\": \"number\",\n                \"example\": 2\n              }\n            }\n          }\n        },\n        \"serial_numbers\": {\n          \"type\": \"string\",\n          \"nullable\": true,\n          \"description\": \"Serial number(s) for this NCR.\",\n          \"example\": \"SN123456\"\n        }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-ncr-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: Ncr
---
