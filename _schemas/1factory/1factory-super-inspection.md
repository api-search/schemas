---
description: SuperInspection schema from 1Factory API
layout: schema
name: SuperInspection
properties_list:
- description: ''
  name: ID
  type: object
- description: ''
  name: insp_ident_1
  type: object
- description: ''
  name: insp_ident_2
  type: object
- description: ''
  name: insp_ident_3
  type: object
- description: ''
  name: part_number
  type: object
- description: ''
  name: rev
  type: object
- description: ''
  name: part_description
  type: object
- description: ''
  name: operation
  type: object
- description: ''
  name: customer_name
  type: object
- description: ''
  name: supplier_name
  type: object
- description: ''
  name: supplier_number
  type: object
- description: ''
  name: project_identifier
  type: object
- description: Location where inspection was performed, from your organization's Site LOV.
  name: site
  type: string
- description: ''
  name: created_by_name
  type: object
- description: ''
  name: created_on
  type: object
- description: Percentage of in-spec parts for this inspection.
  name: in_spec_pct
  type: number
- description: Current status of inspection.
  name: inspection_status
  type: string
- description: Name of user that last set inspection status.
  name: inspected_by_name
  type: string
- description: Date & time that inspection status set.
  name: inspected_on
  type: string
- description: Current review status of inspection.
  name: review_status
  type: string
- description: Name of user that set review status.
  name: reviewed_by_name
  type: string
- description: Date & time that review status was set.
  name: reviewed_on
  type: string
- description: Comments on this inspection
  name: notes
  type: string
- description: 'List of NCR #s associated with this inspection'
  name: ncrs
  type: array
- description: ''
  name: updated_on
  type: object
- description: ''
  name: closed_on
  type: object
provider_name: 1Factory
provider_slug: 1factory
schema_file: json-schema/1factory-super-inspection-schema.json
slug: 1factory-super-inspection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-super-inspection-schema.json\",\n  \"title\": \"SuperInspection\",\n  \"description\": \"SuperInspection schema from 1Factory API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ID\": {\n      \"$ref\": \"#/components/schemas/ID\"\n    },\n    \"insp_ident_1\": {\n      \"$ref\": \"#/components/schemas/insp_ident_1\"\n    },\n    \"insp_ident_2\": {\n      \"$ref\": \"#/components/schemas/insp_ident_2\"\n    },\n    \"insp_ident_3\": {\n      \"$ref\": \"#/components/schemas/insp_ident_3\"\n    },\n    \"part_number\": {\n      \"$ref\": \"#/components/schemas/part_number\"\n    },\n    \"rev\": {\n      \"$ref\": \"#/components/schemas/rev\"\n    },\n    \"part_description\": {\n      \"$ref\": \"#/components/schemas/part_description\"\n    },\n    \"operation\": {\n      \"$ref\": \"#/components/schemas/operation\"\
  \n    },\n    \"customer_name\": {\n      \"$ref\": \"#/components/schemas/customer_name\"\n    },\n    \"supplier_name\": {\n      \"$ref\": \"#/components/schemas/supplier_name\"\n    },\n    \"supplier_number\": {\n      \"$ref\": \"#/components/schemas/supplier_number\"\n    },\n    \"project_identifier\": {\n      \"$ref\": \"#/components/schemas/project_identifier\"\n    },\n    \"site\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Location where inspection was performed, from your organization's Site LOV.\",\n      \"example\": \"QC Lab\"\n    },\n    \"created_by_name\": {\n      \"$ref\": \"#/components/schemas/created_by_username\"\n    },\n    \"created_on\": {\n      \"$ref\": \"#/components/schemas/created_on\"\n    },\n    \"in_spec_pct\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"nullable\": false,\n      \"description\": \"Percentage of in-spec parts for this inspection.\",\n      \"readOnly\": false,\n\
  \      \"minimum\": 0.0,\n      \"maximum\": 100.0,\n      \"example\": 100.0\n    },\n    \"inspection_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Pending\",\n        \"Accepted\",\n        \"Rejected\"\n      ],\n      \"description\": \"Current status of inspection.\",\n      \"default\": \"Accepted\"\n    },\n    \"inspected_by_name\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Name of user that last set inspection status.\",\n      \"example\": \"Will Stallard\"\n    },\n    \"inspected_on\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"format\": \"date-time\",\n      \"description\": \"Date & time that inspection status set.\",\n      \"example\": \"2021-07-16T17:42:31-08:00\"\n    },\n    \"review_status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Pending\",\n        \"Reviewed\"\n      ],\n      \"description\": \"Current review status of inspection.\",\n      \"default\"\
  : \"Pending\"\n    },\n    \"reviewed_by_name\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"description\": \"Name of user that set review status.\",\n      \"example\": \"Nipun Girotra\"\n    },\n    \"reviewed_on\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"format\": \"date-time\",\n      \"description\": \"Date & time that review status was set.\",\n      \"example\": \"2021-07-16T17:53:41-08:00\"\n    },\n    \"notes\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"maxLength\": 32000,\n      \"description\": \"Comments on this inspection\",\n      \"example\": \"Parts are discolored.\"\n    },\n    \"ncrs\": {\n      \"type\": \"array\",\n      \"minItems\": 0,\n      \"items\": {\n        \"type\": \"string\",\n        \"nullable\": false\n      },\n      \"description\": \"List of NCR #s associated with this inspection\",\n      \"example\": [\n        \"NCR-123\",\n        \"NCR-456\"\n      ]\n    },\n    \"updated_on\"\
  : {\n      \"$ref\": \"#/components/schemas/updated_on\"\n    },\n    \"closed_on\": {\n      \"$ref\": \"#/components/schemas/closed_on\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/json-schema/1factory-super-inspection-schema.json
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
title: SuperInspection
---
