---
description: DescribeGroupResponse schema from AWS IAM Identity Center
layout: schema
name: DescribeGroupResponse
properties_list:
- description: ''
  name: GroupId
  type: object
- description: ''
  name: DisplayName
  type: object
- description: ''
  name: ExternalIds
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: IdentityStoreId
  type: object
provider_name: Amazon IAM Identity Center
provider_slug: amazon-iam-identity-center
schema_file: json-schema/identitystore-describe-group-response-schema.json
slug: identitystore-describe-group-response
source_filename: identitystore-describe-group-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-describe-group-response-schema.json\",\n  \"title\": \"DescribeGroupResponse\",\n  \"description\": \"DescribeGroupResponse schema from AWS IAM Identity Center\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GroupId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceId\"\n        },\n        {\n          \"description\": \"The identifier for a group in the identity store.\"\n        }\n      ]\n    },\n    \"DisplayName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroupDisplayName\"\n        },\n        {\n          \"description\": \"The group\\u2019s display name value. The length limit is 1,024 characters. This value can consist of letters, accented characters, symbols, numbers, punctuation, tab,\
  \ new line, carriage return, space, and nonbreaking space in this attribute. This value is specified at the time that the group is created and stored as an attribute of the group object in the identity store.\"\n        }\n      ]\n    },\n    \"ExternalIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalIds\"\n        },\n        {\n          \"description\": \"A list of <code>ExternalId</code> objects that contains the identifiers issued to this resource by an external identity provider.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SensitiveStringType\"\n        },\n        {\n          \"description\": \"A string containing a description of the group.\"\n        }\n      ]\n    },\n    \"IdentityStoreId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityStoreId\"\n        },\n        {\n          \"description\": \"The globally\
  \ unique identifier for the identity store.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GroupId\",\n    \"IdentityStoreId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iam-identity-center/refs/heads/main/json-schema/identitystore-describe-group-response-schema.json
tags:
- Access Control
- Authentication
- AWS
- Identity Management
- Single Sign-On
title: DescribeGroupResponse
---
