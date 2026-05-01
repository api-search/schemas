---
description: The current status of an Elasticsearch domain.
layout: schema
name: ElasticsearchDomainStatus
properties_list:
- description: ''
  name: DomainId
  type: object
- description: ''
  name: DomainName
  type: object
- description: ''
  name: ARN
  type: object
- description: ''
  name: Created
  type: object
- description: ''
  name: Deleted
  type: object
- description: ''
  name: Endpoint
  type: object
- description: ''
  name: Endpoints
  type: object
- description: ''
  name: Processing
  type: object
- description: ''
  name: UpgradeProcessing
  type: object
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
  name: ServiceSoftwareOptions
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
schema_file: json-schema/openapi-elasticsearch-domain-status-schema.json
slug: openapi-elasticsearch-domain-status
source_filename: openapi-elasticsearch-domain-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-elasticsearch-domain-status-schema.json\",\n  \"title\": \"ElasticsearchDomainStatus\",\n  \"description\": \"The current status of an Elasticsearch domain.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DomainId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainId\"\n        },\n        {\n          \"description\": \"The unique identifier for the specified Elasticsearch domain.\"\n        }\n      ]\n    },\n    \"DomainName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainName\"\n        },\n        {\n          \"description\": \"The name of an Elasticsearch domain. Domain names are unique across the domains owned by an account within an AWS region. Domain names start with a letter or number and can contain\
  \ the following characters: a-z (lowercase), 0-9, and - (hyphen).\"\n        }\n      ]\n    },\n    \"ARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"The Amazon resource name (ARN) of an Elasticsearch domain. See <a href=\\\"http://docs.aws.amazon.com/IAM/latest/UserGuide/index.html?Using_Identifiers.html\\\" target=\\\"_blank\\\">Identifiers for IAM Entities</a> in <i>Using AWS Identity and Access Management</i> for more information.\"\n        }\n      ]\n    },\n    \"Created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"The domain creation status. <code>True</code> if the creation of an Elasticsearch domain is complete. <code>False</code> if domain creation is still in progress.\"\n        }\n      ]\n    },\n    \"Deleted\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\
  \n        },\n        {\n          \"description\": \"The domain deletion status. <code>True</code> if a delete request has been received for the domain but resource cleanup is still in progress. <code>False</code> if the domain has not been deleted. Once domain deletion is complete, the status of the domain is no longer returned.\"\n        }\n      ]\n    },\n    \"Endpoint\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceUrl\"\n        },\n        {\n          \"description\": \"The Elasticsearch domain endpoint that you use to submit index and search requests.\"\n        }\n      ]\n    },\n    \"Endpoints\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EndpointsMap\"\n        },\n        {\n          \"description\": \"Map containing the Elasticsearch domain endpoints used to submit index and search requests. Example <code>key, value</code>: <code>'vpc','vpc-endpoint-h2dsd34efgyghrtguk5gt6j2foh4.us-east-1.es.amazonaws.com'</code>.\"\
  \n        }\n      ]\n    },\n    \"Processing\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"The status of the Elasticsearch domain configuration. <code>True</code> if Amazon Elasticsearch Service is processing configuration changes. <code>False</code> if the configuration is active.\"\n        }\n      ]\n    },\n    \"UpgradeProcessing\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"The status of an Elasticsearch domain version upgrade. <code>True</code> if Amazon Elasticsearch Service is undergoing a version upgrade. <code>False</code> if the configuration is active.\"\n        }\n      ]\n    },\n    \"ElasticsearchVersion\": {\n      \"$ref\": \"#/components/schemas/ElasticsearchVersionString\"\n    },\n    \"ElasticsearchClusterConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\":\
  \ \"#/components/schemas/ElasticsearchClusterConfig\"\n        },\n        {\n          \"description\": \"The type and number of instances in the domain cluster.\"\n        }\n      ]\n    },\n    \"EBSOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EBSOptions\"\n        },\n        {\n          \"description\": \"The <code>EBSOptions</code> for the specified domain. See <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-createupdatedomains.html#es-createdomain-configure-ebs\\\" target=\\\"_blank\\\">Configuring EBS-based Storage</a> for more information.\"\n        }\n      ]\n    },\n    \"AccessPolicies\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PolicyDocument\"\n        },\n        {\n          \"description\": \" IAM access policy as a JSON-formatted string.\"\n        }\n      ]\n    },\n    \"SnapshotOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/SnapshotOptions\"\n        },\n        {\n          \"description\": \"Specifies the status of the <code>SnapshotOptions</code>\"\n        }\n      ]\n    },\n    \"VPCOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VPCDerivedInfo\"\n        },\n        {\n          \"description\": \"The <code>VPCOptions</code> for the specified domain. For more information, see <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-vpc.html\\\" target=\\\"_blank\\\">VPC Endpoints for Amazon Elasticsearch Service Domains</a>.\"\n        }\n      ]\n    },\n    \"CognitoOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CognitoOptions\"\n        },\n        {\n          \"description\": \"The <code>CognitoOptions</code> for the specified domain. For more information, see <a href=\\\"http://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-cognito-auth.html\\\"\
  \ target=\\\"_blank\\\">Amazon Cognito Authentication for Kibana</a>.\"\n        }\n      ]\n    },\n    \"EncryptionAtRestOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EncryptionAtRestOptions\"\n        },\n        {\n          \"description\": \" Specifies the status of the <code>EncryptionAtRestOptions</code>.\"\n        }\n      ]\n    },\n    \"NodeToNodeEncryptionOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NodeToNodeEncryptionOptions\"\n        },\n        {\n          \"description\": \"Specifies the status of the <code>NodeToNodeEncryptionOptions</code>.\"\n        }\n      ]\n    },\n    \"AdvancedOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdvancedOptions\"\n        },\n        {\n          \"description\": \"Specifies the status of the <code>AdvancedOptions</code>\"\n        }\n      ]\n    },\n    \"LogPublishingOptions\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/LogPublishingOptions\"\n        },\n        {\n          \"description\": \"Log publishing options for the given domain.\"\n        }\n      ]\n    },\n    \"ServiceSoftwareOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServiceSoftwareOptions\"\n        },\n        {\n          \"description\": \"The current status of the Elasticsearch domain's service software.\"\n        }\n      ]\n    },\n    \"DomainEndpointOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DomainEndpointOptions\"\n        },\n        {\n          \"description\": \"The current status of the Elasticsearch domain's endpoint options.\"\n        }\n      ]\n    },\n    \"AdvancedSecurityOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AdvancedSecurityOptions\"\n        },\n        {\n          \"description\": \"The current status of the Elasticsearch\
  \ domain's advanced security options.\"\n        }\n      ]\n    },\n    \"AutoTuneOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutoTuneOptionsOutput\"\n        },\n        {\n          \"description\": \"The current status of the Elasticsearch domain's Auto-Tune options.\"\n        }\n      ]\n    },\n    \"ChangeProgressDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChangeProgressDetails\"\n        },\n        {\n          \"description\": \"Specifies change details of the domain configuration change.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DomainId\",\n    \"DomainName\",\n    \"ARN\",\n    \"ElasticsearchClusterConfig\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-elasticsearch-domain-status-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: ElasticsearchDomainStatus
---
