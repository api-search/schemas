---
description: PutOrganizationConformancePackRequest schema
layout: schema
name: PutOrganizationConformancePackRequest
properties_list:
- description: ''
  name: OrganizationConformancePackName
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
  name: ExcludedAccounts
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-put-organization-conformance-pack-request-schema.json
slug: config-put-organization-conformance-pack-request
source_filename: config-put-organization-conformance-pack-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-organization-conformance-pack-request-schema.json\",\n  \"title\": \"PutOrganizationConformancePackRequest\",\n  \"description\": \"PutOrganizationConformancePackRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConformancePackName\"\n        },\n        {\n          \"description\": \"Name of the organization conformance pack you want to create.\"\n        }\n      ]\n    },\n    \"TemplateS3Uri\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateS3Uri\"\n        },\n        {\n          \"description\": \"<p>Location of file containing the template body. The uri must point to the conformance pack template (max size:\
  \ 300 KB).</p> <note> <p>You must have access to read Amazon S3 bucket.</p> </note>\"\n        }\n      ]\n    },\n    \"TemplateBody\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TemplateBody\"\n        },\n        {\n          \"description\": \"A string containing full conformance pack template body. Structure containing the template body with a minimum length of 1 byte and a maximum length of 51,200 bytes.\"\n        }\n      ]\n    },\n    \"DeliveryS3Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryS3Bucket\"\n        },\n        {\n          \"description\": \"<p>The name of the Amazon S3 bucket where Config stores conformance pack templates.</p> <note> <p>This field is optional. If used, it must be prefixed with <code>awsconfigconforms</code>.</p> </note>\"\n        }\n      ]\n    },\n    \"DeliveryS3KeyPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryS3KeyPrefix\"\
  \n        },\n        {\n          \"description\": \"<p>The prefix for the Amazon S3 bucket.</p> <note> <p>This field is optional.</p> </note>\"\n        }\n      ]\n    },\n    \"ConformancePackInputParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackInputParameters\"\n        },\n        {\n          \"description\": \"A list of <code>ConformancePackInputParameter</code> objects.\"\n        }\n      ]\n    },\n    \"ExcludedAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExcludedAccounts\"\n        },\n        {\n          \"description\": \"A list of Amazon Web Services accounts to be excluded from an organization conformance pack while deploying a conformance pack.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OrganizationConformancePackName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-put-organization-conformance-pack-request-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: PutOrganizationConformancePackRequest
---
