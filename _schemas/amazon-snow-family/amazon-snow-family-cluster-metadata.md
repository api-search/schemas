---
description: Contains metadata about a specific cluster.
layout: schema
name: ClusterMetadata
properties_list:
- description: ''
  name: ClusterId
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: KmsKeyARN
  type: object
- description: ''
  name: RoleARN
  type: object
- description: ''
  name: ClusterState
  type: object
- description: ''
  name: JobType
  type: object
- description: ''
  name: SnowballType
  type: object
- description: ''
  name: CreationDate
  type: object
- description: ''
  name: Resources
  type: object
- description: ''
  name: AddressId
  type: object
- description: ''
  name: ShippingOption
  type: object
- description: ''
  name: Notification
  type: object
- description: ''
  name: ForwardingAddressId
  type: object
- description: ''
  name: TaxDocuments
  type: object
- description: ''
  name: OnDeviceServiceConfiguration
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-cluster-metadata-schema.json
slug: amazon-snow-family-cluster-metadata
source_filename: amazon-snow-family-cluster-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-cluster-metadata-schema.json\",\n  \"title\": \"ClusterMetadata\",\n  \"description\": \"Contains metadata about a specific cluster.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ClusterId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The automatically generated ID for a cluster.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The optional description of the cluster.\"\n        }\n      ]\n    },\n    \"KmsKeyARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyARN\"\n        },\n        {\n        \
  \  \"description\": \"The <code>KmsKeyARN</code> Amazon Resource Name (ARN) associated with this cluster. This ARN was created using the <a href=\\\"https://docs.aws.amazon.com/kms/latest/APIReference/API_CreateKey.html\\\">CreateKey</a> API action in Key Management Service (KMS.\"\n        }\n      ]\n    },\n    \"RoleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleARN\"\n        },\n        {\n          \"description\": \"The role ARN associated with this cluster. This ARN was created using the <a href=\\\"https://docs.aws.amazon.com/IAM/latest/APIReference/API_CreateRole.html\\\">CreateRole</a> API action in Identity and Access Management (IAM).\"\n        }\n      ]\n    },\n    \"ClusterState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterState\"\n        },\n        {\n          \"description\": \"The current status of the cluster.\"\n        }\n      ]\n    },\n    \"JobType\": {\n      \"allOf\": [\n\
  \        {\n          \"$ref\": \"#/components/schemas/JobType\"\n        },\n        {\n          \"description\": \"The type of job for this cluster. Currently, the only job type supported for clusters is <code>LOCAL_USE</code>.\"\n        }\n      ]\n    },\n    \"SnowballType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnowballType\"\n        },\n        {\n          \"description\": \"<p>The type of Snowcone device to use for this cluster. </p> <note> <p>For cluster jobs, Amazon Web Services Snow Family currently supports only the <code>EDGE</code> device type.</p> </note>\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The creation date for this cluster.\"\n        }\n      ]\n    },\n    \"Resources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobResource\"\n     \
  \   },\n        {\n          \"description\": \"The arrays of <a>JobResource</a> objects that can include updated <a>S3Resource</a> objects or <a>LambdaResource</a> objects.\"\n        }\n      ]\n    },\n    \"AddressId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressId\"\n        },\n        {\n          \"description\": \"The automatically generated ID for a specific address.\"\n        }\n      ]\n    },\n    \"ShippingOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShippingOption\"\n        },\n        {\n          \"description\": \"<p>The shipping speed for each node in this cluster. This speed doesn't dictate how soon you'll get each device, rather it represents how quickly each device moves to its destination while in transit. Regional shipping speeds are as follows:</p> <ul> <li> <p>In Australia, you have access to express shipping. Typically, devices shipped express are delivered in about a day.</p>\
  \ </li> <li> <p>In the European Union (EU), you have access to express shipping. Typically, Snow devices shipped express are delivered in about a day. In addition, most countries in the EU have access to standard shipping, which typically takes less than a week, one way.</p> </li> <li> <p>In India, Snow devices are delivered in one to seven days.</p> </li> <li> <p>In the US, you have access to one-day shipping and two-day shipping.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Notification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Notification\"\n        },\n        {\n          \"description\": \"The Amazon Simple Notification Service (Amazon SNS) notification settings for this cluster.\"\n        }\n      ]\n    },\n    \"ForwardingAddressId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressId\"\n        },\n        {\n          \"description\": \"The ID of the address that you want a cluster shipped to,\
  \ after it will be shipped to its primary address. This field is not supported in most regions.\"\n        }\n      ]\n    },\n    \"TaxDocuments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaxDocuments\"\n        },\n        {\n          \"description\": \"The tax documents required in your Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"OnDeviceServiceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OnDeviceServiceConfiguration\"\n        },\n        {\n          \"description\": \"Represents metadata and configuration settings for services on an Amazon Web Services Snow Family device.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-cluster-metadata-schema.json
tags:
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: ClusterMetadata
---
