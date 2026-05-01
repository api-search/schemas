---
description: A Department of Veterans Affairs facility, including health, benefits, vet center, and cemetery locations.
layout: schema
name: VA Facility
properties_list:
- description: Stable identifier (e.g. vha_688, vba_306, nca_001)
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Department of Veterans Affairs (VA)
provider_slug: department-of-veterans-affairs
schema_file: json-schema/va-facility-schema.json
slug: va-facility
source_filename: va-facility-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.com/department-of-veterans-affairs/schemas/facility.json\",\n  \"title\": \"VA Facility\",\n  \"description\": \"A Department of Veterans Affairs facility, including health, benefits, vet center, and cemetery locations.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"type\", \"attributes\"],\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Stable identifier (e.g. vha_688, vba_306, nca_001)\" },\n    \"type\": { \"type\": \"string\", \"const\": \"facility\" },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"required\": [\"name\", \"facilityType\", \"lat\", \"long\"],\n      \"properties\": {\n        \"name\": { \"type\": \"string\" },\n        \"facilityType\": {\n          \"type\": \"string\",\n          \"enum\": [\"va_health_facility\", \"va_benefits_facility\", \"va_cemetery\", \"vet_center\"]\n        },\n        \"\
  classification\": { \"type\": [\"string\", \"null\"] },\n        \"website\": { \"type\": [\"string\", \"null\"], \"format\": \"uri\" },\n        \"lat\": { \"type\": \"number\", \"minimum\": -90, \"maximum\": 90 },\n        \"long\": { \"type\": \"number\", \"minimum\": -180, \"maximum\": 180 },\n        \"timeZone\": { \"type\": \"string\" },\n        \"address\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"mailing\": { \"$ref\": \"#/$defs/Address\" },\n            \"physical\": { \"$ref\": \"#/$defs/Address\" }\n          }\n        },\n        \"phone\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"main\": { \"type\": [\"string\", \"null\"] },\n            \"fax\": { \"type\": [\"string\", \"null\"] },\n            \"afterHours\": { \"type\": [\"string\", \"null\"] },\n            \"patientAdvocate\": { \"type\": [\"string\", \"null\"] },\n            \"mentalHealthClinic\": { \"type\": [\"string\", \"null\"] },\n\
  \            \"enrollmentCoordinator\": { \"type\": [\"string\", \"null\"] },\n            \"pharmacy\": { \"type\": [\"string\", \"null\"] }\n          }\n        },\n        \"hours\": { \"type\": \"object\", \"additionalProperties\": { \"type\": \"string\" } },\n        \"services\": { \"type\": \"object\" },\n        \"visn\": { \"type\": [\"string\", \"null\"] }\n      }\n    }\n  },\n  \"$defs\": {\n    \"Address\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"address1\": { \"type\": [\"string\", \"null\"] },\n        \"address2\": { \"type\": [\"string\", \"null\"] },\n        \"address3\": { \"type\": [\"string\", \"null\"] },\n        \"city\": { \"type\": [\"string\", \"null\"] },\n        \"state\": { \"type\": [\"string\", \"null\"], \"pattern\": \"^[A-Z]{2}$\" },\n        \"zip\": { \"type\": [\"string\", \"null\"] }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/department-of-veterans-affairs/refs/heads/main/json-schema/va-facility-schema.json
tags:
- Federal Government
- Healthcare
- Veterans
title: VA Facility
---
