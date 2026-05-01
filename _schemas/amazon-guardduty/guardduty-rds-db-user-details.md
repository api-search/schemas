---
description: Contains information about the user and authentication details for a database instance involved in the finding.
layout: schema
name: RdsDbUserDetails
properties_list:
- description: ''
  name: User
  type: object
- description: ''
  name: Application
  type: object
- description: ''
  name: Database
  type: object
- description: ''
  name: Ssl
  type: object
- description: ''
  name: AuthMethod
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-rds-db-user-details-schema.json
slug: guardduty-rds-db-user-details
source_filename: guardduty-rds-db-user-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-rds-db-user-details-schema.json\",\n  \"title\": \"RdsDbUserDetails\",\n  \"description\": \"Contains information about the user and authentication details for a database instance involved in the finding.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"User\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"user\"\n          },\n          \"description\": \"The user name used in the anomalous login attempt.\"\n        }\n      ]\n    },\n    \"Application\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"application\"\n          },\n          \"description\": \"The application\
  \ name used in the anomalous login attempt.\"\n        }\n      ]\n    },\n    \"Database\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"database\"\n          },\n          \"description\": \"The name of the database instance involved in the anomalous login attempt.\"\n        }\n      ]\n    },\n    \"Ssl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"ssl\"\n          },\n          \"description\": \"The version of the Secure Socket Layer (SSL) used for the network.\"\n        }\n      ]\n    },\n    \"AuthMethod\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"authMethod\"\n          },\n          \"description\": \"The authentication method used by the user\
  \ involved in the finding.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-rds-db-user-details-schema.json
tags:
- Anomaly Detection
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: RdsDbUserDetails
---
