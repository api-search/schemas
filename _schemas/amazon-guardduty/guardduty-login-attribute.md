---
description: Information about the login attempts.
layout: schema
name: LoginAttribute
properties_list:
- description: ''
  name: User
  type: object
- description: ''
  name: Application
  type: object
- description: ''
  name: FailedLoginAttempts
  type: object
- description: ''
  name: SuccessfulLoginAttempts
  type: object
provider_name: Amazon GuardDuty
provider_slug: amazon-guardduty
schema_file: json-schema/guardduty-login-attribute-schema.json
slug: guardduty-login-attribute
source_filename: guardduty-login-attribute-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-login-attribute-schema.json\",\n  \"title\": \"LoginAttribute\",\n  \"description\": \"Information about the login attempts.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"User\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"user\"\n          },\n          \"description\": \"Indicates the user name which attempted to log in.\"\n        }\n      ]\n    },\n    \"Application\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"application\"\n          },\n          \"description\": \"Indicates the application name used to attempt log in.\"\n        }\n      ]\n    },\n  \
  \  \"FailedLoginAttempts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"failedLoginAttempts\"\n          },\n          \"description\": \"Represents the sum of failed (unsuccessful) login attempts made to establish a connection to the database instance.\"\n        }\n      ]\n    },\n    \"SuccessfulLoginAttempts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"xml\": {\n            \"name\": \"successfulLoginAttempts\"\n          },\n          \"description\": \"Represents the sum of successful connections (a correct combination of login attributes) made to the database instance by the actor.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-guardduty/refs/heads/main/json-schema/guardduty-login-attribute-schema.json
tags:
- Anomaly Detection
- AWS
- Compliance
- Machine Learning
- Monitoring
- Security
- Threat Detection
title: LoginAttribute
---
