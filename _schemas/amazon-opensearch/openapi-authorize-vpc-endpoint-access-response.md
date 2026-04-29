---
description: Container for response parameters to the <code><a>AuthorizeVpcEndpointAccess</a></code> operation. Contains the account ID and the type of the account being authorized to access the VPC endpoint.
layout: schema
name: AuthorizeVpcEndpointAccessResponse
properties_list:
- description: ''
  name: AuthorizedPrincipal
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-authorize-vpc-endpoint-access-response-schema.json
slug: openapi-authorize-vpc-endpoint-access-response
source_filename: openapi-authorize-vpc-endpoint-access-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-authorize-vpc-endpoint-access-response-schema.json\",\n  \"title\": \"AuthorizeVpcEndpointAccessResponse\",\n  \"description\": \"Container for response parameters to the <code><a>AuthorizeVpcEndpointAccess</a></code> operation. Contains the account ID and the type of the account being authorized to access the VPC endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AuthorizedPrincipal\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AuthorizedPrincipal\"\n        },\n        {\n          \"description\": \"Information about the account or service that was provided access to the domain.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AuthorizedPrincipal\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-authorize-vpc-endpoint-access-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: AuthorizeVpcEndpointAccessResponse
---
