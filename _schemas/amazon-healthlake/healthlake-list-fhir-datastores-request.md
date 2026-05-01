---
description: ''
layout: schema
name: ListFHIRDatastoresRequest
properties_list:
- description: ''
  name: Filter
  type: object
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
provider_name: Amazon HealthLake
provider_slug: amazon-healthlake
schema_file: json-schema/healthlake-list-fhir-datastores-request-schema.json
slug: healthlake-list-fhir-datastores-request
source_filename: healthlake-list-fhir-datastores-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-list-fhir-datastores-request-schema.json\",\n  \"title\": \"ListFHIRDatastoresRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DatastoreFilter\"\n        },\n        {\n          \"description\": \"Lists all filters associated with a FHIR data store request.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"Fetches the next page of data stores when results are paginated.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResultsInteger\"\n        },\n        {\n         \
  \ \"description\": \"The maximum number of data stores returned in a single page of a ListFHIRDatastoresRequest call.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-healthlake/refs/heads/main/json-schema/healthlake-list-fhir-datastores-request-schema.json
tags:
- FHIR
- Health Data
- Healthcare
- HIPAA
- Cloud Computing
title: ListFHIRDatastoresRequest
---
