---
description: An organization conformance pack that has information about conformance packs that Config creates in member accounts.
layout: schema
name: OrganizationConformancePack
properties_list:
- description: ''
  name: OrganizationConformancePackName
  type: object
- description: ''
  name: OrganizationConformancePackArn
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
- description: ''
  name: LastUpdateTime
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-organization-conformance-pack-schema.json
slug: config-organization-conformance-pack
source_filename: config-organization-conformance-pack-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-conformance-pack-schema.json\",\n  \"title\": \"OrganizationConformancePack\",\n  \"description\": \"An organization conformance pack that has information about conformance packs that Config creates in member accounts. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OrganizationConformancePackName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OrganizationConformancePackName\"\n        },\n        {\n          \"description\": \"The name you assign to an organization conformance pack.\"\n        }\n      ]\n    },\n    \"OrganizationConformancePackArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringWithCharLimit256\"\n        },\n        {\n          \"description\": \"Amazon Resource Name (ARN) of organization\
  \ conformance pack.\"\n        }\n      ]\n    },\n    \"DeliveryS3Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryS3Bucket\"\n        },\n        {\n          \"description\": \"<p>The name of the Amazon S3 bucket where Config stores conformance pack templates. </p> <note> <p>This field is optional.</p> </note>\"\n        }\n      ]\n    },\n    \"DeliveryS3KeyPrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryS3KeyPrefix\"\n        },\n        {\n          \"description\": \"<p>Any folder structure you want to add to an Amazon S3 bucket.</p> <note> <p>This field is optional.</p> </note>\"\n        }\n      ]\n    },\n    \"ConformancePackInputParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConformancePackInputParameters\"\n        },\n        {\n          \"description\": \"A list of <code>ConformancePackInputParameter</code> objects.\"\n        }\n  \
  \    ]\n    },\n    \"ExcludedAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExcludedAccounts\"\n        },\n        {\n          \"description\": \"A comma-separated list of accounts excluded from organization conformance pack.\"\n        }\n      ]\n    },\n    \"LastUpdateTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Date\"\n        },\n        {\n          \"description\": \"Last time when organization conformation pack was updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OrganizationConformancePackName\",\n    \"OrganizationConformancePackArn\",\n    \"LastUpdateTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-organization-conformance-pack-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: OrganizationConformancePack
---
