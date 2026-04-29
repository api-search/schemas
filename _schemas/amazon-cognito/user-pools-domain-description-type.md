---
description: A container for information about a domain.
layout: schema
name: DomainDescriptionType
properties_list:
- description: ''
  name: UserPoolId
  type: object
- description: ''
  name: AWSAccountId
  type: object
- description: ''
  name: Domain
  type: object
- description: ''
  name: S3Bucket
  type: object
- description: ''
  name: CloudFrontDistribution
  type: object
- description: ''
  name: Version
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: CustomDomainConfig
  type: object
provider_name: Amazon Cognito
provider_slug: amazon-cognito
schema_file: json-schema/user-pools-domain-description-type-schema.json
slug: user-pools-domain-description-type
source_filename: user-pools-domain-description-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-domain-description-type-schema.json\",\n  \"title\": \"DomainDescriptionType\",\n  \"description\": \"A container for information about a domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserPoolId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserPoolIdType\"\n        },\n        {\n          \"description\": \"The user pool ID.\"\n        }\n      ]\n    },\n    \"AWSAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AWSAccountIdType\"\n        },\n        {\n          \"description\": \"The Amazon Web Services ID for the user pool owner.\"\n        }\n      ]\n    },\n    \"Domain\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainType\"\n        },\n        {\n      \
  \    \"description\": \"The domain string. For custom domains, this is the fully-qualified domain name, such as <code>auth.example.com</code>. For Amazon Cognito prefix domains, this is the prefix alone, such as <code>auth</code>.\"\n        }\n      ]\n    },\n    \"S3Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3BucketType\"\n        },\n        {\n          \"description\": \"The Amazon S3 bucket where the static files for this domain are stored.\"\n        }\n      ]\n    },\n    \"CloudFrontDistribution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The Amazon CloudFront endpoint that you use as the target of the alias that you set up with your Domain Name Service (DNS) provider.\"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainVersionType\"\n        },\n     \
  \   {\n          \"description\": \"The app version.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainStatusType\"\n        },\n        {\n          \"description\": \"The domain status.\"\n        }\n      ]\n    },\n    \"CustomDomainConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomDomainConfigType\"\n        },\n        {\n          \"description\": \"The configuration for a custom domain that hosts the sign-up and sign-in webpages for your application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cognito/refs/heads/main/json-schema/user-pools-domain-description-type-schema.json
tags:
- Authentication
- AWS
- Identity
- OAuth
- User Management
title: DomainDescriptionType
---
