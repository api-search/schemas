---
description: Complaint schema from 1Factory API
layout: schema
name: Complaint
properties_list: []
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-complaint-schema.json
slug: 1factory-complaint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-complaint-schema.json\",\n  \"title\": \"Complaint\",\n  \"description\": \"Complaint schema from 1Factory API\",\n  \"type\": \"object\",\n  \"allOf\": [\n    {\n      \"$ref\": \"#/components/schemas/Issue\"\n    },\n    {\n      \"properties\": {\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"Source of the complaint.\",\n          \"enum\": [\n            \"Customer\",\n            \"Field\"\n          ]\n        },\n        \"customer_address\": {\n          \"type\": \"string\"\n        },\n        \"contact_first_name\": {\n          \"type\": \"string\"\n        },\n        \"contact_last_name\": {\n          \"type\": \"string\"\n        },\n        \"contact_email\": {\n          \"type\": \"string\"\n        },\n        \"contact_phone\": {\n         \
  \ \"type\": \"string\"\n        },\n        \"customer_ncr_no\": {\n          \"type\": \"string\",\n          \"description\": \"Customer NCR number if available.\"\n        },\n        \"rma_no\": {\n          \"type\": \"string\"\n        },\n        \"device_identifier\": {\n          \"type\": \"string\"\n        },\n        \"serial_nos\": {\n          \"type\": \"string\"\n        },\n        \"capa_required\": {\n          \"type\": \"boolean\"\n        },\n        \"capa_id\": {\n          \"type\": \"number\"\n        },\n        \"date_due\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Date & time that a Complaint is due.\",\n          \"example\": \"2021-07-21T07:14:42-08:00\"\n        },\n        \"complaint_on\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Date & time of the original complaint.\",\n          \"example\": \"2021-07-21T07:14:42-08:00\"\n   \
  \     }\n      }\n    }\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-complaint-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: Complaint
---
