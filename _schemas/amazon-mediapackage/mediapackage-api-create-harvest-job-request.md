---
description: Configuration parameters used to create a new HarvestJob.
layout: schema
name: CreateHarvestJobRequest
properties_list:
- description: ''
  name: EndTime
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: OriginEndpointId
  type: object
- description: ''
  name: S3Destination
  type: object
- description: ''
  name: StartTime
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-create-harvest-job-request-schema.json
slug: mediapackage-api-create-harvest-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-create-harvest-job-request-schema.json\",\n  \"title\": \"CreateHarvestJobRequest\",\n  \"description\": \"Configuration parameters used to create a new HarvestJob.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"endTime\"\n          },\n          \"description\": \"The end of the time-window which will be harvested\\n\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The ID of the HarvestJob. The ID must be unique\
  \ within the region\\nand it cannot be changed after the HarvestJob is submitted\\n\"\n        }\n      ]\n    },\n    \"OriginEndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"originEndpointId\"\n          },\n          \"description\": \"The ID of the OriginEndpoint that the HarvestJob will harvest from.\\nThis cannot be changed after the HarvestJob is submitted.\\n\"\n        }\n      ]\n    },\n    \"S3Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Destination\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"s3Destination\"\n          }\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"startTime\"\n          },\n          \"description\": \"\
  The start of the time-window which will be harvested\\n\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"S3Destination\",\n    \"EndTime\",\n    \"OriginEndpointId\",\n    \"StartTime\",\n    \"Id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-create-harvest-job-request-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: CreateHarvestJobRequest
---
