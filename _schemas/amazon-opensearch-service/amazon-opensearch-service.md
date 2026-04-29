---
description: Schema defining the structure of an Amazon OpenSearch Service domain resource, including cluster configuration, storage options, access policies, encryption settings, and VPC configuration.
layout: schema
name: Amazon OpenSearch Service Domain Definition
properties_list:
- description: The unique identifier for the OpenSearch domain.
  name: DomainId
  type: string
- description: The name of the OpenSearch domain.
  name: DomainName
  type: string
- description: The Amazon Resource Name of the domain.
  name: ARN
  type: string
- description: Whether the domain creation is complete.
  name: Created
  type: boolean
- description: Whether the domain is being deleted.
  name: Deleted
  type: boolean
- description: The domain endpoint used to submit index, search, and data upload requests.
  name: Endpoint
  type: string
- description: Map of VPC endpoints for the domain.
  name: Endpoints
  type: object
- description: The version of OpenSearch or Elasticsearch running on the domain.
  name: EngineVersion
  type: string
- description: ''
  name: ClusterConfig
  type: object
- description: ''
  name: EBSOptions
  type: object
- description: IAM access policy as a JSON-formatted string.
  name: AccessPolicies
  type: string
- description: ''
  name: SnapshotOptions
  type: object
- description: ''
  name: VPCOptions
  type: object
- description: ''
  name: EncryptionAtRestOptions
  type: object
- description: ''
  name: NodeToNodeEncryptionOptions
  type: object
- description: Key-value pairs for advanced configuration options.
  name: AdvancedOptions
  type: object
- description: Log publishing options for the domain.
  name: LogPublishingOptions
  type: object
- description: ''
  name: DomainEndpointOptions
  type: object
- description: ''
  name: AutoTuneOptions
  type: object
- description: Tags associated with the domain.
  name: tags
  type: array
provider_name: Amazon OpenSearch Service
provider_slug: amazon-opensearch-service
schema_file: json-schema/amazon-opensearch-service-schema.json
slug: amazon-opensearch-service
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schemas.apievangelist.com/amazon-opensearch-service/domain-definition\",\n  \"title\": \"Amazon OpenSearch Service Domain Definition\",\n  \"description\": \"Schema defining the structure of an Amazon OpenSearch Service domain resource, including cluster configuration, storage options, access policies, encryption settings, and VPC configuration.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"DomainName\"\n  ],\n  \"properties\": {\n    \"DomainId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the OpenSearch domain.\"\n    },\n    \"DomainName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the OpenSearch domain.\",\n      \"minLength\": 3,\n      \"maxLength\": 28,\n      \"pattern\": \"^[a-z][a-z0-9-]+$\"\n    },\n    \"ARN\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name of the domain.\"\
  \n    },\n    \"Created\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain creation is complete.\"\n    },\n    \"Deleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the domain is being deleted.\"\n    },\n    \"Endpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The domain endpoint used to submit index, search, and data upload requests.\"\n    },\n    \"Endpoints\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Map of VPC endpoints for the domain.\"\n    },\n    \"EngineVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The version of OpenSearch or Elasticsearch running on the domain.\"\n    },\n    \"ClusterConfig\": {\n      \"$ref\": \"#/$defs/ClusterConfig\"\n    },\n    \"EBSOptions\": {\n      \"$ref\": \"#/$defs/EBSOptions\"\n    },\n    \"AccessPolicies\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"IAM access policy as a JSON-formatted string.\"\n    },\n    \"SnapshotOptions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"AutomatedSnapshotStartHour\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"maximum\": 23,\n          \"description\": \"The time in UTC format when the service takes a daily automated snapshot.\"\n        }\n      }\n    },\n    \"VPCOptions\": {\n      \"$ref\": \"#/$defs/VPCOptions\"\n    },\n    \"EncryptionAtRestOptions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether encryption at rest is enabled.\"\n        },\n        \"KmsKeyId\": {\n          \"type\": \"string\",\n          \"description\": \"The KMS key ID for encryption at rest.\"\n        }\n      }\n    },\n    \"NodeToNodeEncryptionOptions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Enabled\": {\n          \"type\"\
  : \"boolean\",\n          \"description\": \"Whether node-to-node encryption is enabled.\"\n        }\n      }\n    },\n    \"AdvancedOptions\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Key-value pairs for advanced configuration options.\"\n    },\n    \"LogPublishingOptions\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/$defs/LogPublishingOption\"\n      },\n      \"description\": \"Log publishing options for the domain.\"\n    },\n    \"DomainEndpointOptions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"EnforceHTTPS\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to require HTTPS for all traffic to the domain.\"\n        },\n        \"TLSSecurityPolicy\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"Policy-Min-TLS-1-0-2019-07\",\n            \"Policy-Min-TLS-1-2-2019-07\"\
  ,\n            \"Policy-Min-TLS-1-2-PFS-2023-10\"\n          ],\n          \"description\": \"The minimum TLS security policy.\"\n        },\n        \"CustomEndpointEnabled\": {\n          \"type\": \"boolean\"\n        },\n        \"CustomEndpoint\": {\n          \"type\": \"string\"\n        },\n        \"CustomEndpointCertificateArn\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"AutoTuneOptions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"State\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"ENABLED\",\n            \"DISABLED\",\n            \"ENABLE_IN_PROGRESS\",\n            \"DISABLE_IN_PROGRESS\",\n            \"DISABLED_AND_ROLLBACK_SCHEDULED\",\n            \"DISABLED_AND_ROLLBACK_IN_PROGRESS\",\n            \"DISABLED_AND_ROLLBACK_COMPLETE\",\n            \"DISABLED_AND_ROLLBACK_ERROR\",\n            \"ERROR\"\n          ]\n        },\n        \"DesiredState\": {\n          \"type\": \"string\",\n\
  \          \"enum\": [\n            \"ENABLED\",\n            \"DISABLED\"\n          ]\n        }\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/$defs/Tag\"\n      },\n      \"description\": \"Tags associated with the domain.\"\n    }\n  },\n  \"$defs\": {\n    \"ClusterConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Container for the cluster configuration of an OpenSearch domain.\",\n      \"properties\": {\n        \"InstanceType\": {\n          \"type\": \"string\",\n          \"description\": \"The instance type for data nodes.\"\n        },\n        \"InstanceCount\": {\n          \"type\": \"integer\",\n          \"minimum\": 1,\n          \"description\": \"The number of data nodes in the cluster.\"\n        },\n        \"DedicatedMasterEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether dedicated master nodes are enabled.\"\n        },\n        \"DedicatedMasterType\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"The instance type for dedicated master nodes.\"\n        },\n        \"DedicatedMasterCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of dedicated master nodes.\"\n        },\n        \"ZoneAwarenessEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether zone awareness is enabled.\"\n        },\n        \"WarmEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether UltraWarm storage is enabled.\"\n        },\n        \"WarmType\": {\n          \"type\": \"string\",\n          \"description\": \"The instance type for UltraWarm nodes.\"\n        },\n        \"WarmCount\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of UltraWarm nodes.\"\n        },\n        \"ColdStorageOptions\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Enabled\": {\n              \"type\":\
  \ \"boolean\"\n            }\n          }\n        }\n      }\n    },\n    \"EBSOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Container for EBS-based storage configuration.\",\n      \"properties\": {\n        \"EBSEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether EBS-based storage is enabled.\"\n        },\n        \"VolumeType\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"standard\",\n            \"gp2\",\n            \"gp3\",\n            \"io1\"\n          ],\n          \"description\": \"The type of EBS volume.\"\n        },\n        \"VolumeSize\": {\n          \"type\": \"integer\",\n          \"description\": \"The size of the EBS volume in GiB.\"\n        },\n        \"Iops\": {\n          \"type\": \"integer\",\n          \"description\": \"The baseline I/O performance for the EBS volume.\"\n        },\n        \"Throughput\": {\n          \"type\": \"integer\",\n          \"description\":\
  \ \"The throughput for gp3 volumes in MiB/s.\"\n        }\n      }\n    },\n    \"VPCOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Container for VPC configuration options.\",\n      \"properties\": {\n        \"SubnetIds\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"A list of subnet IDs for VPC endpoints.\"\n        },\n        \"SecurityGroupIds\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"A list of security group IDs for VPC endpoints.\"\n        }\n      }\n    },\n    \"LogPublishingOption\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"CloudWatchLogsLogGroupArn\": {\n          \"type\": \"string\",\n          \"description\": \"The ARN of the CloudWatch Logs group.\"\n        },\n        \"Enabled\": {\n          \"type\": \"boolean\",\n          \"description\"\
  : \"Whether log publishing is enabled.\"\n        }\n      }\n    },\n    \"Tag\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"Key\",\n        \"Value\"\n      ],\n      \"properties\": {\n        \"Key\": {\n          \"type\": \"string\",\n          \"description\": \"The tag key.\",\n          \"minLength\": 1,\n          \"maxLength\": 128\n        },\n        \"Value\": {\n          \"type\": \"string\",\n          \"description\": \"The tag value.\",\n          \"maxLength\": 256\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch-service/refs/heads/main/json-schema/amazon-opensearch-service-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Full-Text Search
- Log Analytics
- OpenSearch
- Search
title: Amazon OpenSearch Service Domain Definition
---
