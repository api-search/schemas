---
description: Returned in response to a successful <code>LookupDeveloperIdentity</code> action.
layout: schema
name: LookupDeveloperIdentityResponse
properties_list:
- description: ''
  name: IdentityId
  type: object
- description: ''
  name: DeveloperUserIdentifierList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Cognito
provider_slug: aws-cognito
schema_file: json-schema/cognito-identity-lookup-developer-identity-response-schema.json
slug: cognito-identity-lookup-developer-identity-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"IdentityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdentityId\"\n        },\n        {\n          \"description\": \"A unique identifier in the format REGION:GUID.\"\n        }\n      ]\n    },\n    \"DeveloperUserIdentifierList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeveloperUserIdentifierList\"\n        },\n        {\n          \"description\": \"This is the list of developer user identifiers associated with an identity ID. Cognito supports the association of multiple developer user identifiers with an identity ID.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationKey\"\n        },\n        {\n          \"description\": \"A pagination token. The first call you make will have <code>NextToken</code> set to null. After that the service will return <code>NextToken</code>\
  \ values as needed. For example, let's say you make a request with <code>MaxResults</code> set to 10, and there are 20 matches in the database. The service will return a pagination token as a part of the response. This token can be used to call the API again and get results starting from the 11th match.\"\n        }\n      ]\n    }\n  },\n  \"description\": \"Returned in response to a successful <code>LookupDeveloperIdentity</code> action.\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-lookup-developer-identity-response-schema.json\",\n  \"title\": \"LookupDeveloperIdentityResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-cognito/refs/heads/main/json-schema/cognito-identity-lookup-developer-identity-response-schema.json
tags:
- Authentication
- Authorization
- AWS
- Identity
- Identity Provider
- OAuth2
- OIDC
title: LookupDeveloperIdentityResponse
---
