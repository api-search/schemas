---
description: The configuration of an Elasticsearch domain.
layout: schema
name: ElasticsearchDomainConfig
properties_list:
- description: ''
  name: ElasticsearchVersion
  type: object
- description: ''
  name: ElasticsearchClusterConfig
  type: object
- description: ''
  name: EBSOptions
  type: object
- description: ''
  name: AccessPolicies
  type: object
- description: ''
  name: SnapshotOptions
  type: object
- description: ''
  name: VPCOptions
  type: object
- description: ''
  name: CognitoOptions
  type: object
- description: ''
  name: EncryptionAtRestOptions
  type: object
- description: ''
  name: NodeToNodeEncryptionOptions
  type: object
- description: ''
  name: AdvancedOptions
  type: object
- description: ''
  name: LogPublishingOptions
  type: object
- description: ''
  name: DomainEndpointOptions
  type: object
- description: ''
  name: AdvancedSecurityOptions
  type: object
- description: ''
  name: AutoTuneOptions
  type: object
- description: ''
  name: ChangeProgressDetails
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-elasticsearch-domain-config-schema.json
slug: openapi-elasticsearch-domain-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-elasticsearch-domain-config-schema.json\",\n  \"title\": \"ElasticsearchDomainConfig\",\n  \"description\": \"The configuration of an Elasticsearch domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ElasticsearchVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ElasticsearchVersionStatus\"\n        },\n        {\n          \"description\": \"String of format X.Y to specify version for the Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"ElasticsearchClusterConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ElasticsearchClusterConfigStatus\"\n        },\n        {\n          \"description\": \"Specifies the <code>ElasticsearchClusterConfig</code> for the Elasticsearch domain.\"\n        }\n      ]\n\
  \    },\n    \"EBSOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EBSOptionsStatus\"\n        },\n        {\n          \"description\": \"Specifies the <code>EBSOptions</code> for the Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"AccessPolicies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccessPoliciesStatus\"\n        },\n        {\n          \"description\": \"IAM access policy as a JSON-formatted string.\"\n        }\n      ]\n    },\n    \"SnapshotOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotOptionsStatus\"\n        },\n        {\n          \"description\": \"Specifies the <code>SnapshotOptions</code> for the Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"VPCOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VPCDerivedInfoStatus\"\n        },\n        {\n          \"description\": \"The <code>VPCOptions</code>\
  \ for the specified domain. For more information, see <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-vpc.html\\\" target=\\\"_blank\\\">VPC Endpoints for Amazon Elasticsearch Service Domains</a>.\"\n        }\n      ]\n    },\n    \"CognitoOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CognitoOptionsStatus\"\n        },\n        {\n          \"description\": \"The <code>CognitoOptions</code> for the specified domain. For more information, see <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-cognito-auth.html\\\" target=\\\"_blank\\\">Amazon Cognito Authentication for Kibana</a>.\"\n        }\n      ]\n    },\n    \"EncryptionAtRestOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionAtRestOptionsStatus\"\n        },\n        {\n          \"description\": \"Specifies the <code>EncryptionAtRestOptions</code> for the Elasticsearch\
  \ domain.\"\n        }\n      ]\n    },\n    \"NodeToNodeEncryptionOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeToNodeEncryptionOptionsStatus\"\n        },\n        {\n          \"description\": \"Specifies the <code>NodeToNodeEncryptionOptions</code> for the Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"AdvancedOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdvancedOptionsStatus\"\n        },\n        {\n          \"description\": \"Specifies the <code>AdvancedOptions</code> for the domain. See <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-createupdatedomains.html#es-createdomain-configure-advanced-options\\\" target=\\\"_blank\\\">Configuring Advanced Options</a> for more information.\"\n        }\n      ]\n    },\n    \"LogPublishingOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogPublishingOptionsStatus\"\
  \n        },\n        {\n          \"description\": \"Log publishing options for the given domain.\"\n        }\n      ]\n    },\n    \"DomainEndpointOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainEndpointOptionsStatus\"\n        },\n        {\n          \"description\": \"Specifies the <code>DomainEndpointOptions</code> for the Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"AdvancedSecurityOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdvancedSecurityOptionsStatus\"\n        },\n        {\n          \"description\": \"Specifies <code>AdvancedSecurityOptions</code> for the domain. \"\n        }\n      ]\n    },\n    \"AutoTuneOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoTuneOptionsStatus\"\n        },\n        {\n          \"description\": \"Specifies <code>AutoTuneOptions</code> for the domain. \"\n        }\n      ]\n    },\n    \"ChangeProgressDetails\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeProgressDetails\"\n        },\n        {\n          \"description\": \"Specifies change details of the domain configuration change.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-elasticsearch-domain-config-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: ElasticsearchDomainConfig
---
