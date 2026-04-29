---
description: This object is a container for common summary information about the change. The summary doesn't contain the whole change structure.
layout: schema
name: ChangeSummary
properties_list:
- description: ''
  name: ChangeType
  type: object
- description: ''
  name: Entity
  type: object
- description: ''
  name: Details
  type: object
- description: ''
  name: ErrorDetailList
  type: object
- description: ''
  name: ChangeName
  type: object
provider_name: Amazon Marketplace
provider_slug: amazon-marketplace
schema_file: json-schema/amazon-marketplace-change-summary-schema.json
slug: amazon-marketplace-change-summary
source_filename: amazon-marketplace-change-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-change-summary-schema.json\",\n  \"title\": \"ChangeSummary\",\n  \"description\": \"This object is a container for common summary information about the change. The summary doesn't contain the whole change structure.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ChangeType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeType\"\n        },\n        {\n          \"description\": \"The type of the change.\"\n        }\n      ]\n    },\n    \"Entity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Entity\"\n        },\n        {\n          \"description\": \"The entity to be changed.\"\n        }\n      ]\n    },\n    \"Details\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Json\"\
  \n        },\n        {\n          \"description\": \"This object contains details specific to the change type of the requested change.\"\n        }\n      ]\n    },\n    \"ErrorDetailList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorDetailList\"\n        },\n        {\n          \"description\": \"An array of <code>ErrorDetail</code> objects associated with the change.\"\n        }\n      ]\n    },\n    \"ChangeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeName\"\n        },\n        {\n          \"description\": \"Optional name for the change.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-marketplace/refs/heads/main/json-schema/amazon-marketplace-change-summary-schema.json
tags:
- AWS
- Commerce
- ISV
- Marketplace
- Software Catalog
title: ChangeSummary
---
