---
description: An object that contains the <code>ChangeType</code>, <code>Details</code>, and <code>Entity</code>.
layout: schema
name: Change
properties_list:
- description: ''
  name: ChangeType
  type: object
- description: ''
  name: Entity
  type: object
- description: ''
  name: EntityTags
  type: object
- description: ''
  name: Details
  type: object
- description: ''
  name: ChangeName
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-change-schema.json
slug: amazon-marketplace-change
source_filename: amazon-marketplace-change-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-change-schema.json\",\n  \"title\": \"Change\",\n  \"description\": \"An object that contains the <code>ChangeType</code>, <code>Details</code>, and <code>Entity</code>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChangeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeType\"\n        },\n        {\n          \"description\": \"Change types are single string values that describe your intention for the change. Each change type is unique for each <code>EntityType</code> provided in the change's scope. For more information on change types available for single-AMI products, see <a href=\\\"https://docs.aws.amazon.com/marketplace-catalog/latest/api-reference/ami-products.html#working-with-single-AMI-products\\\">Working with single-AMI\
  \ products</a>. Also, for more information on change types available for container-based products, see <a href=\\\"https://docs.aws.amazon.com/marketplace-catalog/latest/api-reference/container-products.html#working-with-container-products\\\">Working with container products</a>.\"\n        }\n      ]\n    },\n    \"Entity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Entity\"\n        },\n        {\n          \"description\": \"The entity to be changed.\"\n        }\n      ]\n    },\n    \"EntityTags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags associated with the change.\"\n        }\n      ]\n    },\n    \"Details\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Json\"\n        },\n        {\n          \"description\": \"This object contains details specific to the change type of the requested change. For more information\
  \ on change types available for single-AMI products, see <a href=\\\"https://docs.aws.amazon.com/marketplace-catalog/latest/api-reference/ami-products.html#working-with-single-AMI-products\\\">Working with single-AMI products</a>. Also, for more information on change types available for container-based products, see <a href=\\\"https://docs.aws.amazon.com/marketplace-catalog/latest/api-reference/container-products.html#working-with-container-products\\\">Working with container products</a>.\"\n        }\n      ]\n    },\n    \"ChangeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeName\"\n        },\n        {\n          \"description\": \"Optional name for the change.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ChangeType\",\n    \"Entity\",\n    \"Details\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-change-schema.json
tags:
- AWS
- Commerce
- ISV
- Marketplace
- Software Catalog
title: Change
---
