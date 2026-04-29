---
description: PutConformancePackRequest schema
layout: schema
name: PutConformancePackRequest
properties_list:
- description: ''
  name: ConformancePackName
  type: object
- description: ''
  name: TemplateS3Uri
  type: object
- description: ''
  name: TemplateBody
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
  name: TemplateSSMDocumentDetails
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-conformance-pack-request-schema.json
slug: config-put-conformance-pack-request
source_filename: config-put-conformance-pack-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-conformance-pack-request-schema.json\",\n  \"title\": \"PutConformancePackRequest\",\n  \"description\": \"PutConformancePackRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackName\"\n        },\n        {\n          \"description\": \"The unique name of the conformance pack you want to deploy.\"\n        }\n      ]\n    },\n    \"TemplateS3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateS3Uri\"\n        },\n        {\n          \"description\": \"<p>The location of the file containing the template body (<code>s3://bucketname/prefix</code>). The uri must point to a conformance pack template (max size: 300 KB) that is\
  \ located in an Amazon S3 bucket in the same Region as the conformance pack. </p> <note> <p>You must have access to read Amazon S3 bucket.</p> </note>\"\n        }\n      ]\n    },\n    \"TemplateBody\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateBody\"\n        },\n        {\n          \"description\": \"<p>A string containing the full conformance pack template body. The structure containing the template body has a minimum length of 1 byte and a maximum length of 51,200 bytes.</p> <note> <p>You can use a YAML template with two resource types: Config rule (<code>AWS::Config::ConfigRule</code>) and remediation action (<code>AWS::Config::RemediationConfiguration</code>).</p> </note>\"\n        }\n      ]\n    },\n    \"DeliveryS3Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryS3Bucket\"\n        },\n        {\n          \"description\": \"<p>The name of the Amazon S3 bucket where Config stores conformance\
  \ pack templates.</p> <note> <p>This field is optional.</p> </note>\"\n        }\n      ]\n    },\n    \"DeliveryS3KeyPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryS3KeyPrefix\"\n        },\n        {\n          \"description\": \"<p>The prefix for the Amazon S3 bucket. </p> <note> <p>This field is optional.</p> </note>\"\n        }\n      ]\n    },\n    \"ConformancePackInputParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackInputParameters\"\n        },\n        {\n          \"description\": \"A list of <code>ConformancePackInputParameter</code> objects.\"\n        }\n      ]\n    },\n    \"TemplateSSMDocumentDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateSSMDocumentDetails\"\n        },\n        {\n          \"description\": \"An object of type <code>TemplateSSMDocumentDetails</code>, which contains the name or the Amazon Resource Name\
  \ (ARN) of the Amazon Web Services Systems Manager document (SSM document) and the version of the SSM document that is used to create a conformance pack.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConformancePackName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-conformance-pack-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: PutConformancePackRequest
---
