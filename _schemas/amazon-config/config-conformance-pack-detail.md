---
description: Returns details of a conformance pack. A conformance pack is a collection of Config rules and remediation actions that can be easily deployed in an account and a region.
layout: schema
name: ConformancePackDetail
properties_list:
- description: ''
  name: ConformancePackName
  type: object
- description: ''
  name: ConformancePackArn
  type: object
- description: ''
  name: ConformancePackId
  type: object
- description: ''
  name: DeliveryS3Bucket
  type: object
- description: ''
  name: DeliveryS3KeyPrefix
  type: object
- description: ''
  name: ConformancePackInputParameters
  type: object
- description: ''
  name: LastUpdateRequestedTime
  type: object
- description: ''
  name: CreatedBy
  type: object
- description: ''
  name: TemplateSSMDocumentDetails
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-conformance-pack-detail-schema.json
slug: config-conformance-pack-detail
source_filename: config-conformance-pack-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-detail-schema.json\",\n  \"title\": \"ConformancePackDetail\",\n  \"description\": \"Returns details of a conformance pack. A conformance pack is a collection of Config rules and remediation actions that can be easily deployed in an account and a region.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackName\"\n        },\n        {\n          \"description\": \"Name of the conformance pack.\"\n        }\n      ]\n    },\n    \"ConformancePackArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackArn\"\n        },\n        {\n          \"description\": \"Amazon Resource Name (ARN) of the conformance pack.\"\n        }\n\
  \      ]\n    },\n    \"ConformancePackId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackId\"\n        },\n        {\n          \"description\": \"ID of the conformance pack.\"\n        }\n      ]\n    },\n    \"DeliveryS3Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryS3Bucket\"\n        },\n        {\n          \"description\": \"<p>The name of the Amazon S3 bucket where Config stores conformance pack templates. </p> <note> <p>This field is optional.</p> </note>\"\n        }\n      ]\n    },\n    \"DeliveryS3KeyPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryS3KeyPrefix\"\n        },\n        {\n          \"description\": \"<p>The prefix for the Amazon S3 bucket.</p> <note> <p>This field is optional.</p> </note>\"\n        }\n      ]\n    },\n    \"ConformancePackInputParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackInputParameters\"\
  \n        },\n        {\n          \"description\": \"A list of <code>ConformancePackInputParameter</code> objects.\"\n        }\n      ]\n    },\n    \"LastUpdateRequestedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"The last time a conformation pack update was requested. \"\n        }\n      ]\n    },\n    \"CreatedBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"The Amazon Web Services service that created the conformance pack.\"\n        }\n      ]\n    },\n    \"TemplateSSMDocumentDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateSSMDocumentDetails\"\n        },\n        {\n          \"description\": \"An object that contains the name or Amazon Resource Name (ARN) of the Amazon Web Services Systems Manager document (SSM document)\
  \ and the version of the SSM document that is used to create a conformance pack.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConformancePackName\",\n    \"ConformancePackArn\",\n    \"ConformancePackId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-conformance-pack-detail-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ConformancePackDetail
---
