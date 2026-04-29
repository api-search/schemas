---
description: A HarvestJob resource configuration
layout: schema
name: HarvestJob
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: ChannelId
  type: object
- description: ''
  name: CreatedAt
  type: object
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
- description: ''
  name: Status
  type: object
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
schema_file: json-schema/mediapackage-api-harvest-job-schema.json
slug: mediapackage-api-harvest-job
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-harvest-job-schema.json\",\n  \"title\": \"HarvestJob\",\n  \"description\": \"A HarvestJob resource configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"The Amazon Resource Name (ARN) assigned to the HarvestJob.\\n\"\n        }\n      ]\n    },\n    \"ChannelId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"channelId\"\n          },\n          \"description\": \"The ID of the Channel that the HarvestJob will harvest from.\\n\"\n        }\n \
  \     ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"createdAt\"\n          },\n          \"description\": \"The date and time the HarvestJob was submitted.\\n\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"endTime\"\n          },\n          \"description\": \"The end of the time-window which will be harvested.\\n\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The ID of the HarvestJob. The ID must be unique within the region\\nand it cannot be changed after the HarvestJob is submitted.\\n\"\n\
  \        }\n      ]\n    },\n    \"OriginEndpointId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"originEndpointId\"\n          },\n          \"description\": \"The ID of the OriginEndpoint that the HarvestJob will harvest from.\\nThis cannot be changed after the HarvestJob is submitted.\\n\"\n        }\n      ]\n    },\n    \"S3Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Destination\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"s3Destination\"\n          }\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"startTime\"\n          },\n          \"description\": \"The start of the time-window which will be harvested.\\n\"\n        }\n      ]\n    },\n\
  \    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Status\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"status\"\n          },\n          \"description\": \"The current status of the HarvestJob. Consider setting up a CloudWatch Event to listen for\\nHarvestJobs as they succeed or fail. In the event of failure, the CloudWatch Event will\\ninclude an explanation of why the HarvestJob failed.\\n\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediapackage/refs/heads/main/json-schema/mediapackage-api-harvest-job-schema.json
tags:
- AWS
- Broadcasting
- Media Processing
- Media
title: HarvestJob
---
