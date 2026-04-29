---
description: Container for request parameters to the <code><a>AuthorizeVpcEndpointAccess</a></code> operation. Specifies the account to be permitted to manage VPC endpoints against the domain.
layout: schema
name: AuthorizeVpcEndpointAccessRequest
properties_list:
- description: ''
  name: Account
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-authorize-vpc-endpoint-access-request-schema.json
slug: openapi-authorize-vpc-endpoint-access-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-authorize-vpc-endpoint-access-request-schema.json\",\n  \"title\": \"AuthorizeVpcEndpointAccessRequest\",\n  \"description\": \"Container for request parameters to the <code><a>AuthorizeVpcEndpointAccess</a></code> operation. Specifies the account to be permitted to manage VPC endpoints against the domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Account\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AWSAccount\"\n        },\n        {\n          \"description\": \"The account ID to grant access to.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Account\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-authorize-vpc-endpoint-access-request-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: AuthorizeVpcEndpointAccessRequest
---
