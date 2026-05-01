---
description: Container for the parameters to the <code><a>UpdateElasticsearchDomain</a></code> operation. Specifies the type and number of instances in the domain cluster.
layout: schema
name: UpdateElasticsearchDomainConfigRequest
properties_list:
- description: ''
  name: ElasticsearchClusterConfig
  type: object
- description: ''
  name: EBSOptions
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
  name: AdvancedOptions
  type: object
- description: ''
  name: AccessPolicies
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
  name: NodeToNodeEncryptionOptions
  type: object
- description: ''
  name: EncryptionAtRestOptions
  type: object
- description: ''
  name: AutoTuneOptions
  type: object
- description: ''
  name: DryRun
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-update-elasticsearch-domain-config-request-schema.json
slug: openapi-update-elasticsearch-domain-config-request
source_filename: openapi-update-elasticsearch-domain-config-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-update-elasticsearch-domain-config-request-schema.json\",\n  \"title\": \"UpdateElasticsearchDomainConfigRequest\",\n  \"description\": \"Container for the parameters to the <code><a>UpdateElasticsearchDomain</a></code> operation. Specifies the type and number of instances in the domain cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ElasticsearchClusterConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ElasticsearchClusterConfig\"\n        },\n        {\n          \"description\": \"The type and number of instances to instantiate for the domain cluster.\"\n        }\n      ]\n    },\n    \"EBSOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EBSOptions\"\n        },\n        {\n          \"description\"\
  : \"Specify the type and size of the EBS volume that you want to use. \"\n        }\n      ]\n    },\n    \"SnapshotOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnapshotOptions\"\n        },\n        {\n          \"description\": \"Option to set the time, in UTC format, for the daily automated snapshot. Default value is <code>0</code> hours. \"\n        }\n      ]\n    },\n    \"VPCOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VPCOptions\"\n        },\n        {\n          \"description\": \"Options to specify the subnets and security groups for VPC endpoint. For more information, see <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-vpc.html#es-creating-vpc\\\" target=\\\"_blank\\\">Creating a VPC</a> in <i>VPC Endpoints for Amazon Elasticsearch Service Domains</i>\"\n        }\n      ]\n    },\n    \"CognitoOptions\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/CognitoOptions\"\n        },\n        {\n          \"description\": \"Options to specify the Cognito user and identity pools for Kibana authentication. For more information, see <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-cognito-auth.html\\\" target=\\\"_blank\\\">Amazon Cognito Authentication for Kibana</a>.\"\n        }\n      ]\n    },\n    \"AdvancedOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdvancedOptions\"\n        },\n        {\n          \"description\": \"Modifies the advanced option to allow references to indices in an HTTP request body. Must be <code>false</code> when configuring access to individual sub-resources. By default, the value is <code>true</code>. See <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-createupdatedomains.html#es-createdomain-configure-advanced-options\\\" target=\\\"_blank\\\">Configuration Advanced\
  \ Options</a> for more information.\"\n        }\n      ]\n    },\n    \"AccessPolicies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyDocument\"\n        },\n        {\n          \"description\": \"IAM access policy as a JSON-formatted string.\"\n        }\n      ]\n    },\n    \"LogPublishingOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogPublishingOptions\"\n        },\n        {\n          \"description\": \"Map of <code>LogType</code> and <code>LogPublishingOption</code>, each containing options to publish a given type of Elasticsearch log.\"\n        }\n      ]\n    },\n    \"DomainEndpointOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainEndpointOptions\"\n        },\n        {\n          \"description\": \"Options to specify configuration that will be applied to the domain endpoint.\"\n        }\n      ]\n    },\n    \"AdvancedSecurityOptions\": {\n    \
  \  \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdvancedSecurityOptionsInput\"\n        },\n        {\n          \"description\": \"Specifies advanced security options.\"\n        }\n      ]\n    },\n    \"NodeToNodeEncryptionOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeToNodeEncryptionOptions\"\n        },\n        {\n          \"description\": \"Specifies the NodeToNodeEncryptionOptions.\"\n        }\n      ]\n    },\n    \"EncryptionAtRestOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionAtRestOptions\"\n        },\n        {\n          \"description\": \"Specifies the Encryption At Rest Options.\"\n        }\n      ]\n    },\n    \"AutoTuneOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoTuneOptions\"\n        },\n        {\n          \"description\": \"Specifies Auto-Tune options.\"\n        }\n      ]\n    },\n    \"DryRun\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DryRun\"\n        },\n        {\n          \"description\": \" This flag, when set to True, specifies whether the <code>UpdateElasticsearchDomain</code> request should return the results of validation checks without actually applying the change. This flag, when set to True, specifies the deployment mechanism through which the update shall be applied on the domain. This will not actually perform the Update. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-update-elasticsearch-domain-config-request-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: UpdateElasticsearchDomainConfigRequest
---
