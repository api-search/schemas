---
description: 'Specifies the current status of the VPC endpoint: <ul> <li>CREATING: Indicates that the VPC endpoint is currently being created.</li> <li>CREATE_FAILED: Indicates that the VPC endpoint creation failed.</li> <li>ACTIVE: Indicates that the VPC endpoint is currently active.</li> <li>UPDATING: Indicates that the VPC endpoint is currently being updated.</li> <li>UPDATE_FAILED: Indicates that the VPC endpoint update failed.</li> <li>DELETING: Indicates that the VPC endpoint is currently being deleted.</li> <li>DELETE_FAILED: Indicates that the VPC endpoint deletion failed.</li> </ul>'
layout: schema
name: VpcEndpointStatus
properties_list: []
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-vpc-endpoint-status-schema.json
slug: openapi-vpc-endpoint-status
source_filename: openapi-vpc-endpoint-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-vpc-endpoint-status-schema.json\",\n  \"title\": \"VpcEndpointStatus\",\n  \"description\": \"Specifies the current status of the VPC endpoint: <ul> <li>CREATING: Indicates that the VPC endpoint is currently being created.</li> <li>CREATE_FAILED: Indicates that the VPC endpoint creation failed.</li> <li>ACTIVE: Indicates that the VPC endpoint is currently active.</li> <li>UPDATING: Indicates that the VPC endpoint is currently being updated.</li> <li>UPDATE_FAILED: Indicates that the VPC endpoint update failed.</li> <li>DELETING: Indicates that the VPC endpoint is currently being deleted.</li> <li>DELETE_FAILED: Indicates that the VPC endpoint deletion failed.</li> </ul> \",\n  \"type\": \"string\",\n  \"enum\": [\n    \"CREATING\",\n    \"CREATE_FAILED\",\n    \"ACTIVE\",\n    \"UPDATING\",\n\
  \    \"UPDATE_FAILED\",\n    \"DELETING\",\n    \"DELETE_FAILED\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-vpc-endpoint-status-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: VpcEndpointStatus
---
