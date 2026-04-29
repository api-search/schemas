---
description: Contains information about the finding, which is generated when abnormal or suspicious activity is detected.
layout: schema
name: Finding
properties_list:
- description: ''
  name: AccountId
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: Confidence
  type: object
- description: ''
  name: CreatedAt
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: Id
  type: object
- description: ''
  name: Partition
  type: object
- description: ''
  name: Region
  type: object
- description: ''
  name: Resource
  type: object
- description: ''
  name: SchemaVersion
  type: object
- description: ''
  name: Service
  type: object
- description: ''
  name: Severity
  type: object
- description: ''
  name: Title
  type: object
- description: ''
  name: Type
  type: object
- description: ''
  name: UpdatedAt
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-finding-schema.json
slug: guardduty-finding
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-finding-schema.json\",\n  \"title\": \"Finding\",\n  \"description\": \"Contains information about the finding, which is generated when abnormal or suspicious activity is detected.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"accountId\"\n          },\n          \"description\": \"The ID of the account in which the finding was generated.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"arn\"\n          },\n          \"description\": \"The ARN of the finding.\"\n    \
  \    }\n      ]\n    },\n    \"Confidence\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"confidence\"\n          },\n          \"description\": \"The confidence score for the finding.\"\n        }\n      ]\n    },\n    \"CreatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"createdAt\"\n          },\n          \"description\": \"The time and date when the finding was created.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"description\"\n          },\n          \"description\": \"The description of the finding.\"\n        }\n      ]\n    },\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"id\"\n          },\n          \"description\": \"The ID of the finding.\"\n        }\n      ]\n    },\n    \"Partition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"partition\"\n          },\n          \"description\": \"The partition associated with the finding.\"\n        }\n      ]\n    },\n    \"Region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"region\"\n          },\n          \"description\": \"The Region where the finding was generated.\"\n        }\n      ]\n    },\n    \"Resource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Resource\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"resource\"\n\
  \          }\n        }\n      ]\n    },\n    \"SchemaVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"schemaVersion\"\n          },\n          \"description\": \"The version of the schema used for the finding.\"\n        }\n      ]\n    },\n    \"Service\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Service\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"service\"\n          }\n        }\n      ]\n    },\n    \"Severity\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"severity\"\n          },\n          \"description\": \"The severity of the finding.\"\n        }\n      ]\n    },\n    \"Title\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n\
  \          \"xml\": {\n            \"name\": \"title\"\n          },\n          \"description\": \"The title of the finding.\"\n        }\n      ]\n    },\n    \"Type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingType\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"type\"\n          },\n          \"description\": \"The type of finding.\"\n        }\n      ]\n    },\n    \"UpdatedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"updatedAt\"\n          },\n          \"description\": \"The time and date when the finding was last updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AccountId\",\n    \"Arn\",\n    \"CreatedAt\",\n    \"Id\",\n    \"Region\",\n    \"Resource\",\n    \"SchemaVersion\",\n    \"Severity\",\n    \"Type\",\n    \"UpdatedAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-finding-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: Finding
---
