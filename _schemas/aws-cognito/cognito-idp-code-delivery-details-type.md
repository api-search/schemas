---
description: The delivery details for an email or SMS message that Amazon Cognito sent for authentication or verification.
layout: schema
name: CodeDeliveryDetailsType
properties_list:
- description: ''
  name: Destination
  type: object
- description: ''
  name: DeliveryMedium
  type: object
- description: ''
  name: AttributeName
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-code-delivery-details-type-schema.json
slug: cognito-idp-code-delivery-details-type
source_filename: cognito-idp-code-delivery-details-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Destination\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringType\"\n        },\n        {\n          \"description\": \"The email address or phone number destination where Amazon Cognito sent the code.\"\n        }\n      ]\n    },\n    \"DeliveryMedium\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeliveryMediumType\"\n        },\n        {\n          \"description\": \"The method that Amazon Cognito used to send the code.\"\n        }\n      ]\n    },\n    \"AttributeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeNameType\"\n        },\n        {\n          \"description\": \"The name of the attribute that Amazon Cognito verifies with the code.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"The delivery details for an email or SMS message that Amazon Cognito sent for authentication or verification.\"\
  ,\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-code-delivery-details-type-schema.json\",\n  \"title\": \"CodeDeliveryDetailsType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-code-delivery-details-type-schema.json
tags:
- Authentication
- Authorization
- Identity
- Identity Provider
- OAuth2
- OIDC
title: CodeDeliveryDetailsType
---
