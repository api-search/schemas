---
description: Provides the details of a finding.
layout: schema
name: Finding
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: archived
  type: object
- description: ''
  name: category
  type: object
- description: ''
  name: classificationDetails
  type: object
- description: ''
  name: count
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: id
  type: object
- description: ''
  name: partition
  type: object
- description: ''
  name: policyDetails
  type: object
- description: ''
  name: region
  type: object
- description: ''
  name: resourcesAffected
  type: object
- description: ''
  name: sample
  type: object
- description: ''
  name: schemaVersion
  type: object
- description: ''
  name: severity
  type: object
- description: ''
  name: title
  type: object
- description: ''
  name: type
  type: object
- description: ''
  name: updatedAt
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-finding-schema.json
slug: amazon-macie-finding
source_filename: amazon-macie-finding-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-finding-schema.json\",\n  \"title\": \"Finding\",\n  \"description\": \"Provides the details of a finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the Amazon Web Services account that the finding applies to. This is typically the account that owns the affected resource.\"\n        }\n      ]\n    },\n    \"archived\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the finding is archived (suppressed).\"\n        }\n      ]\n    },\n    \"category\": {\n      \"allOf\": [\n        {\n     \
  \     \"$ref\": \"#/components/schemas/FindingCategory\"\n        },\n        {\n          \"description\": \"The category of the finding. Possible values are: CLASSIFICATION, for a sensitive data finding; and, POLICY, for a policy finding.\"\n        }\n      ]\n    },\n    \"classificationDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClassificationDetails\"\n        },\n        {\n          \"description\": \"The details of a sensitive data finding. This value is null for a policy finding.\"\n        }\n      ]\n    },\n    \"count\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__long\"\n        },\n        {\n          \"description\": \"The total number of occurrences of the finding. For sensitive data findings, this value is always 1. All sensitive data findings are considered unique.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\
  \n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when Amazon Macie created the finding.\"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The description of the finding.\"\n        }\n      ]\n    },\n    \"id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The unique identifier for the finding. This is a random string that Amazon Macie generates and assigns to a finding when it creates the finding.\"\n        }\n      ]\n    },\n    \"partition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Web Services partition that Amazon Macie created the finding in.\"\n        }\n      ]\n    },\n\
  \    \"policyDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyDetails\"\n        },\n        {\n          \"description\": \"The details of a policy finding. This value is null for a sensitive data finding.\"\n        }\n      ]\n    },\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region that Amazon Macie created the finding in.\"\n        }\n      ]\n    },\n    \"resourcesAffected\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourcesAffected\"\n        },\n        {\n          \"description\": \"The resources that the finding applies to.\"\n        }\n      ]\n    },\n    \"sample\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__boolean\"\n        },\n        {\n          \"description\": \"Specifies whether the finding is a sample finding.\
  \ A <i>sample finding</i> is a finding that uses example data to demonstrate what a finding might contain.\"\n        }\n      ]\n    },\n    \"schemaVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The version of the schema that was used to define the data structures in the finding.\"\n        }\n      ]\n    },\n    \"severity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Severity\"\n        },\n        {\n          \"description\": \"The severity level and score for the finding.\"\n        }\n      ]\n    },\n    \"title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"The brief description of the finding.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingType\"\n        },\n \
  \       {\n          \"description\": \"The type of the finding.\"\n        }\n      ]\n    },\n    \"updatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__timestampIso8601\"\n        },\n        {\n          \"description\": \"The date and time, in UTC and extended ISO 8601 format, when Amazon Macie last updated the finding. For sensitive data findings, this value is the same as the value for the createdAt property. All sensitive data findings are considered new.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-finding-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: Finding
---
