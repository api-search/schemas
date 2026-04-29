---
description: ''
layout: schema
name: AddRawMaterialCompostQuantity
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: typeName
  type: string
- description: ''
  name: quantityValue
  type: object
provider_name: AgStack Foundation
provider_slug: agstack
schema_file: json-schema/agstack-openagri-farm-calendar-addrawmaterialcompostquantity-schema.json
slug: agstack-openagri-farm-calendar-addrawmaterialcompostquantity
source_filename: agstack-openagri-farm-calendar-addrawmaterialcompostquantity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://agstack.org/schemas/AddRawMaterialCompostQuantity.json\",\n  \"title\": \"AddRawMaterialCompostQuantity\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"readOnly\": true\n    },\n    \"typeName\": {\n      \"type\": \"string\"\n    },\n    \"quantityValue\": {\n      \"$ref\": \"#/components/schemas/AppliedAmmountField\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"quantityValue\",\n    \"typeName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agstack/refs/heads/main/json-schema/agstack-openagri-farm-calendar-addrawmaterialcompostquantity-schema.json
tags:
- Agriculture
- Linux Foundation
- Open Source
- Geospatial
- Precision Agriculture
- Linked Data
title: AddRawMaterialCompostQuantity
---
