---
description: Options to configure endpoint for the Elasticsearch domain.
layout: schema
name: DomainEndpointOptions
properties_list:
- description: ''
  name: EnforceHTTPS
  type: object
- description: ''
  name: TLSSecurityPolicy
  type: object
- description: ''
  name: CustomEndpointEnabled
  type: object
- description: ''
  name: CustomEndpoint
  type: object
- description: ''
  name: CustomEndpointCertificateArn
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-domain-endpoint-options-schema.json
slug: openapi-domain-endpoint-options
source_filename: openapi-domain-endpoint-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-domain-endpoint-options-schema.json\",\n  \"title\": \"DomainEndpointOptions\",\n  \"description\": \"Options to configure endpoint for the Elasticsearch domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"EnforceHTTPS\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specify if only HTTPS endpoint should be enabled for the Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"TLSSecurityPolicy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TLSSecurityPolicy\"\n        },\n        {\n          \"description\": \"Specify the TLS security policy that needs to be applied to the HTTPS endpoint of Elasticsearch domain. <br/> It can be one of the following values:\
  \ <ul> <li><b>Policy-Min-TLS-1-0-2019-07: </b> TLS security policy which supports TLSv1.0 and higher.</li> <li><b>Policy-Min-TLS-1-2-2019-07: </b> TLS security policy which supports only TLSv1.2</li> </ul> \"\n        }\n      ]\n    },\n    \"CustomEndpointEnabled\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Specify if custom endpoint should be enabled for the Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"CustomEndpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainNameFqdn\"\n        },\n        {\n          \"description\": \"Specify the fully qualified domain for your custom endpoint.\"\n        }\n      ]\n    },\n    \"CustomEndpointCertificateArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"Specify ACM certificate ARN for your custom endpoint.\"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-domain-endpoint-options-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DomainEndpointOptions
---
