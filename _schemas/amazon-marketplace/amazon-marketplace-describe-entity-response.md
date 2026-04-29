---
description: DescribeEntityResponse schema from Amazon Marketplace API
layout: schema
name: DescribeEntityResponse
properties_list:
- description: ''
  name: EntityType
  type: object
- description: ''
  name: EntityIdentifier
  type: object
- description: ''
  name: EntityArn
  type: object
- description: ''
  name: LastModifiedDate
  type: object
- description: ''
  name: Details
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-describe-entity-response-schema.json
slug: amazon-marketplace-describe-entity-response
source_filename: amazon-marketplace-describe-entity-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-describe-entity-response-schema.json\",\n  \"title\": \"DescribeEntityResponse\",\n  \"description\": \"DescribeEntityResponse schema from Amazon Marketplace API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EntityType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EntityType\"\n        },\n        {\n          \"description\": \"The named type of the entity, in the format of <code>EntityType@Version</code>.\"\n        }\n      ]\n    },\n    \"EntityIdentifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Identifier\"\n        },\n        {\n          \"description\": \"The identifier of the entity, in the format of <code>EntityId@RevisionId</code>.\"\n        }\n      ]\n    },\n    \"EntityArn\": {\n \
  \     \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The ARN associated to the unique identifier for the entity referenced in this request.\"\n        }\n      ]\n    },\n    \"LastModifiedDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DateTimeISO8601\"\n        },\n        {\n          \"description\": \"The last modified date of the entity, in ISO 8601 format (2018-02-27T13:45:22Z).\"\n        }\n      ]\n    },\n    \"Details\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Json\"\n        },\n        {\n          \"description\": \"This stringified JSON object includes the details of the entity.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-describe-entity-response-schema.json
tags:
- AWS
- Commerce
- ISV
- Marketplace
- Software Catalog
title: DescribeEntityResponse
---
