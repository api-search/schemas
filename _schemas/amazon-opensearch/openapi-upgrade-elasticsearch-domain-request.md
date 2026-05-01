---
description: Container for request parameters to <code> <a>UpgradeElasticsearchDomain</a> </code> operation.
layout: schema
name: UpgradeElasticsearchDomainRequest
properties_list:
- description: ''
  name: DomainName
  type: object
- description: ''
  name: TargetVersion
  type: object
- description: ''
  name: PerformCheckOnly
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-upgrade-elasticsearch-domain-request-schema.json
slug: openapi-upgrade-elasticsearch-domain-request
source_filename: openapi-upgrade-elasticsearch-domain-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-upgrade-elasticsearch-domain-request-schema.json\",\n  \"title\": \"UpgradeElasticsearchDomainRequest\",\n  \"description\": \" Container for request parameters to <code> <a>UpgradeElasticsearchDomain</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainName\": {\n      \"$ref\": \"#/components/schemas/DomainName\"\n    },\n    \"TargetVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ElasticsearchVersionString\"\n        },\n        {\n          \"description\": \"The version of Elasticsearch that you intend to upgrade the domain to.\"\n        }\n      ]\n    },\n    \"PerformCheckOnly\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\"\
  : \" This flag, when set to True, indicates that an Upgrade Eligibility Check needs to be performed. This will not actually perform the Upgrade. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DomainName\",\n    \"TargetVersion\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-upgrade-elasticsearch-domain-request-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: UpgradeElasticsearchDomainRequest
---
