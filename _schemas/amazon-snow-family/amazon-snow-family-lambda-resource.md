---
description: Identifies
layout: schema
name: LambdaResource
properties_list:
- description: ''
  name: LambdaArn
  type: object
- description: ''
  name: EventTriggers
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-lambda-resource-schema.json
slug: amazon-snow-family-lambda-resource
source_filename: amazon-snow-family-lambda-resource-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-lambda-resource-schema.json\",\n  \"title\": \"LambdaResource\",\n  \"description\": \"Identifies \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LambdaArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"An Amazon Resource Name (ARN) that represents an Lambda function to be triggered by PUT object actions on the associated local Amazon S3 resource.\"\n        }\n      ]\n    },\n    \"EventTriggers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventTriggerDefinitionList\"\n        },\n        {\n          \"description\": \"The array of ARNs for <a>S3Resource</a> objects to trigger the <a>LambdaResource</a> objects associated with this job.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-lambda-resource-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: LambdaResource
---
