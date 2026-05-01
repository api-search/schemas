---
description: Container for response parameters to the <code><a>ListVpcEndpointAccess</a></code> operation. Returns a list of accounts id and account type authorized to manage VPC endpoints.
layout: schema
name: ListVpcEndpointAccessResponse
properties_list:
- description: ''
  name: AuthorizedPrincipalList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-list-vpc-endpoint-access-response-schema.json
slug: openapi-list-vpc-endpoint-access-response
source_filename: openapi-list-vpc-endpoint-access-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-vpc-endpoint-access-response-schema.json\",\n  \"title\": \"ListVpcEndpointAccessResponse\",\n  \"description\": \"Container for response parameters to the <code><a>ListVpcEndpointAccess</a></code> operation. Returns a list of accounts id and account type authorized to manage VPC endpoints.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuthorizedPrincipalList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthorizedPrincipalList\"\n        },\n        {\n          \"description\": \"List of <code>AuthorizedPrincipal</code> describing the details of the permissions to manage VPC endpoints against the specified domain.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\
  \n        },\n        {\n          \"description\": \"Provides an identifier to allow retrieval of paginated results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AuthorizedPrincipalList\",\n    \"NextToken\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-vpc-endpoint-access-response-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: ListVpcEndpointAccessResponse
---
