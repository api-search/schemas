---
description: Provides information about the type and other characteristics of an entity that performed an action on an affected resource.
layout: schema
name: UserIdentity
properties_list:
- description: ''
  name: assumedRole
  type: object
- description: ''
  name: awsAccount
  type: object
- description: ''
  name: awsService
  type: object
- description: ''
  name: federatedUser
  type: object
- description: ''
  name: iamUser
  type: object
- description: ''
  name: root
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon Macie
provider_slug: amazon-macie
schema_file: json-schema/amazon-macie-user-identity-schema.json
slug: amazon-macie-user-identity
source_filename: amazon-macie-user-identity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-user-identity-schema.json\",\n  \"title\": \"UserIdentity\",\n  \"description\": \"Provides information about the type and other characteristics of an entity that performed an action on an affected resource.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assumedRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AssumedRole\"\n        },\n        {\n          \"description\": \"If the action was performed with temporary security credentials that were obtained using the AssumeRole operation of the Security Token Service (STS) API, the identifiers, session context, and other details about the identity.\"\n        }\n      ]\n    },\n    \"awsAccount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsAccount\"\n        },\n\
  \        {\n          \"description\": \"If the action was performed using the credentials for another Amazon Web Services account, the details of that account.\"\n        }\n      ]\n    },\n    \"awsService\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsService\"\n        },\n        {\n          \"description\": \"If the action was performed by an Amazon Web Services account that belongs to an Amazon Web Service, the name of the service.\"\n        }\n      ]\n    },\n    \"federatedUser\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FederatedUser\"\n        },\n        {\n          \"description\": \"If the action was performed with temporary security credentials that were obtained using the GetFederationToken operation of the Security Token Service (STS) API, the identifiers, session context, and other details about the identity.\"\n        }\n      ]\n    },\n    \"iamUser\": {\n      \"allOf\": [\n        {\n \
  \         \"$ref\": \"#/components/schemas/IamUser\"\n        },\n        {\n          \"description\": \"If the action was performed using the credentials for an Identity and Access Management (IAM) user, the name and other details about the user.\"\n        }\n      ]\n    },\n    \"root\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserIdentityRoot\"\n        },\n        {\n          \"description\": \"If the action was performed using the credentials for your Amazon Web Services account, the details of your account.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserIdentityType\"\n        },\n        {\n          \"description\": \"The type of entity that performed the action.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-macie/refs/heads/main/json-schema/amazon-macie-user-identity-schema.json
tags:
- AWS
- Data Security
- Sensitive Data
- Privacy
- Compliance
- Machine Learning
- S3
title: UserIdentity
---
