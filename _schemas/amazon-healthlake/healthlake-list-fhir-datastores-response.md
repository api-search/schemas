---
description: ''
layout: schema
name: ListFHIRDatastoresResponse
properties_list:
- description: ''
  name: DatastorePropertiesList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-list-fhir-datastores-response-schema.json
slug: healthlake-list-fhir-datastores-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-list-fhir-datastores-response-schema.json\",\n  \"title\": \"ListFHIRDatastoresResponse\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DatastorePropertiesList\"\n  ],\n  \"properties\": {\n    \"DatastorePropertiesList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastorePropertiesList\"\n        },\n        {\n          \"description\": \"All properties associated with the listed data stores.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"Pagination token that can be used to retrieve the next page of results.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-list-fhir-datastores-response-schema.json
tags:
- AWS
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: ListFHIRDatastoresResponse
---
