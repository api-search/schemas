---
description: Contains information about the schema attribute.
layout: schema
name: SchemaAttributeType
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: AttributeDataType
  type: object
- description: ''
  name: DeveloperOnlyAttribute
  type: object
- description: ''
  name: Mutable
  type: object
- description: ''
  name: Required
  type: object
- description: ''
  name: NumberAttributeConstraints
  type: object
- description: ''
  name: StringAttributeConstraints
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-idp-schema-attribute-type-schema.json
slug: cognito-idp-schema-attribute-type
source_filename: cognito-idp-schema-attribute-type-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomAttributeNameType\"\n        },\n        {\n          \"description\": \"A schema attribute of the name type.\"\n        }\n      ]\n    },\n    \"AttributeDataType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AttributeDataType\"\n        },\n        {\n          \"description\": \"The attribute data type.\"\n        }\n      ]\n    },\n    \"DeveloperOnlyAttribute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"<note> <p>You should use <a href=\\\"https://docs.aws.amazon.com/cognito-user-identity-pools/latest/APIReference/API_UserPoolClientType.html#CognitoUserPools-Type-UserPoolClientType-WriteAttributes\\\">WriteAttributes</a> in the user pool client to control how attributes can be mutated for new\
  \ use cases instead of using <code>DeveloperOnlyAttribute</code>.</p> </note> <p>Specifies whether the attribute type is developer only. This attribute can only be modified by an administrator. Users won't be able to modify this attribute using their access token. For example, <code>DeveloperOnlyAttribute</code> can be modified using AdminUpdateUserAttributes but can't be updated using UpdateUserAttributes.</p>\"\n        }\n      ]\n    },\n    \"Mutable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"<p>Specifies whether the value of the attribute can be changed.</p> <p>For any user pool attribute that is mapped to an IdP attribute, you must set this parameter to <code>true</code>. Amazon Cognito updates mapped attributes when users sign in to your application through an IdP. If an attribute is immutable, Amazon Cognito throws an error when it attempts to update the attribute. For more\
  \ information, see <a href=\\\"https://docs.aws.amazon.com/cognito/latest/developerguide/cognito-user-pools-specifying-attribute-mapping.html\\\">Specifying Identity Provider Attribute Mappings for Your User Pool</a>.</p>\"\n        }\n      ]\n    },\n    \"Required\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanType\"\n        },\n        {\n          \"description\": \"Specifies whether a user pool attribute is required. If the attribute is required and the user doesn't provide a value, registration or sign-in will fail.\"\n        }\n      ]\n    },\n    \"NumberAttributeConstraints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NumberAttributeConstraintsType\"\n        },\n        {\n          \"description\": \"Specifies the constraints for an attribute of the number type.\"\n        }\n      ]\n    },\n    \"StringAttributeConstraints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringAttributeConstraintsType\"\
  \n        },\n        {\n          \"description\": \"Specifies the constraints for an attribute of the string type.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Contains information about the schema attribute.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-schema-attribute-type-schema.json\",\n  \"title\": \"SchemaAttributeType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-idp-schema-attribute-type-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: SchemaAttributeType
---
