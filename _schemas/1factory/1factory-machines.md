---
description: List of machines for the inspection. Only for manufacturing inspections. Entries in this list must match the Mfg. Resources - Machines LOV configured for your organization.
layout: schema
name: machines
properties_list: []
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-machines-schema.json
slug: 1factory-machines
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-machines-schema.json\",\n  \"title\": \"machines\",\n  \"description\": \"List of machines for the inspection. Only for manufacturing inspections. Entries in this list must match the Mfg. Resources - Machines LOV configured for your organization.\",\n  \"type\": \"array\",\n  \"items\": {\n    \"type\": \"string\",\n    \"nullable\": false,\n    \"minItems\": 0\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-machines-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: machines
---
