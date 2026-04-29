---
description: ''
layout: schema
name: Data21
properties_list:
- description: ''
  name: zi_c_location_id
  type: integer
- description: ''
  name: zi_es_ecid
  type: integer
- description: ''
  name: zi_es_location_id
  type: string
- description: ''
  name: zi_c_is_hq
  type: string
- description: ''
  name: zi_c_tier_grade
  type: string
- description: ''
  name: zi_c_name
  type: string
- description: ''
  name: zi_c_name_display
  type: string
- description: ''
  name: zi_c_legal_entity_type
  type: string
- description: ''
  name: zi_c_url
  type: string
- description: ''
  name: zi_c_street
  type: string
- description: ''
  name: zi_c_street_2
  type: string
- description: ''
  name: zi_c_city
  type: string
- description: ''
  name: zi_c_state
  type: string
- description: ''
  name: zi_c_zip
  type: string
- description: ''
  name: zi_c_country
  type: string
- description: ''
  name: zi_match_reason
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-data21-schema.json
slug: zoominfo-data21
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"zi_c_location_id\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"zi_es_ecid\": {\n      \"type\": \"integer\",\n      \"example\": 500123\n    },\n    \"zi_es_location_id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"zi_c_is_hq\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"zi_c_tier_grade\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"zi_c_name\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"zi_c_name_display\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"zi_c_legal_entity_type\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"zi_c_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com/resource\"\n    },\n    \"zi_c_street\": {\n     \
  \ \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"zi_c_street_2\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"zi_c_city\": {\n      \"type\": \"string\",\n      \"example\": \"San Francisco\"\n    },\n    \"zi_c_state\": {\n      \"type\": \"string\",\n      \"example\": \"CA\"\n    },\n    \"zi_c_zip\": {\n      \"type\": \"string\",\n      \"example\": \"94105\"\n    },\n    \"zi_c_country\": {\n      \"type\": \"string\",\n      \"example\": \"US\"\n    },\n    \"zi_match_reason\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"zi_match_name\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        },\n        \"zi_match_reason_building_name\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        },\n        \"zi_match_reason_building_number\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n     \
  \   },\n        \"zi_match_reason_business_type\": {\n          \"type\": \"string\",\n          \"example\": \"standard\"\n        },\n        \"zi_match_reason_city\": {\n          \"type\": \"string\",\n          \"example\": \"San Francisco\"\n        },\n        \"zi_match_reason_company_phone\": {\n          \"type\": \"string\",\n          \"example\": \"+1-555-555-1234\"\n        },\n        \"zi_match_reason_country\": {\n          \"type\": \"string\",\n          \"example\": \"US\"\n        },\n        \"zi_match_reason_directional\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"zi_match_reason_name\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        },\n        \"zi_match_reason_road_name\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        },\n        \"zi_match_reason_road_type\": {\n          \"type\": \"string\",\n          \"example\": \"\
  standard\"\n        },\n        \"zi_match_reason_state\": {\n          \"type\": \"string\",\n          \"example\": \"CA\"\n        },\n        \"zi_match_reason_unit\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"zi_match_reason_website\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"zi_match_reason_zip\": {\n          \"type\": \"string\",\n          \"example\": \"94105\"\n        },\n        \"zi_match_score\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"zi_match_name\",\n        \"zi_match_reason_building_name\",\n        \"zi_match_reason_building_number\",\n        \"zi_match_reason_business_type\",\n        \"zi_match_reason_city\",\n        \"zi_match_reason_company_phone\",\n        \"zi_match_reason_country\",\n        \"zi_match_reason_directional\",\n        \"zi_match_reason_name\"\
  ,\n        \"zi_match_reason_road_name\",\n        \"zi_match_reason_road_type\",\n        \"zi_match_reason_state\",\n        \"zi_match_reason_unit\",\n        \"zi_match_reason_website\",\n        \"zi_match_reason_zip\",\n        \"zi_match_score\"\n      ]\n    }\n  },\n  \"required\": [\n    \"zi_c_location_id\",\n    \"zi_es_ecid\",\n    \"zi_es_location_id\",\n    \"zi_c_is_hq\",\n    \"zi_c_tier_grade\",\n    \"zi_c_name\",\n    \"zi_c_name_display\",\n    \"zi_c_legal_entity_type\",\n    \"zi_c_url\",\n    \"zi_c_street\",\n    \"zi_c_street_2\",\n    \"zi_c_city\",\n    \"zi_c_state\",\n    \"zi_c_zip\",\n    \"zi_c_country\",\n    \"zi_match_reason\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Data21\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-data21-schema.json
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
title: Data21
---
