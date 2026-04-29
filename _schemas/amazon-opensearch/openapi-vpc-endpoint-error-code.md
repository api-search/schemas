---
description: 'Specifies the error code of the failure encountered while describing the VPC endpoint: <ul> <li>ENDPOINT_NOT_FOUND: Indicates that the requested VPC endpoint does not exist.</li> <li>SERVER_ERROR: Indicates the describe endpoint operation failed due to an internal server error.</li> </ul>'
layout: schema
name: VpcEndpointErrorCode
properties_list: []
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-vpc-endpoint-error-code-schema.json
slug: openapi-vpc-endpoint-error-code
source_filename: openapi-vpc-endpoint-error-code-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-vpc-endpoint-error-code-schema.json\",\n  \"title\": \"VpcEndpointErrorCode\",\n  \"description\": \"Specifies the error code of the failure encountered while describing the VPC endpoint: <ul> <li>ENDPOINT_NOT_FOUND: Indicates that the requested VPC endpoint does not exist.</li> <li>SERVER_ERROR: Indicates the describe endpoint operation failed due to an internal server error.</li> </ul> \",\n  \"type\": \"string\",\n  \"enum\": [\n    \"ENDPOINT_NOT_FOUND\",\n    \"SERVER_ERROR\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-vpc-endpoint-error-code-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: VpcEndpointErrorCode
---
