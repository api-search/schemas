---
description: CreateClusterRequest schema from Amazon Snow Family API
layout: schema
name: CreateClusterRequest
properties_list:
- description: ''
  name: JobType
  type: object
- description: ''
  name: Resources
  type: object
- description: ''
  name: OnDeviceServiceConfiguration
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: AddressId
  type: object
- description: ''
  name: KmsKeyARN
  type: object
- description: ''
  name: RoleARN
  type: object
- description: ''
  name: SnowballType
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
  name: RemoteManagement
  type: object
- description: ''
  name: InitialClusterSize
  type: object
- description: ''
  name: ForceCreateJobs
  type: object
- description: ''
  name: LongTermPricingIds
  type: object
- description: ''
  name: SnowballCapacityPreference
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-create-cluster-request-schema.json
slug: amazon-snow-family-create-cluster-request
source_filename: amazon-snow-family-create-cluster-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-cluster-request-schema.json\",\n  \"title\": \"CreateClusterRequest\",\n  \"description\": \"CreateClusterRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobType\"\n        },\n        {\n          \"description\": \"<p>The type of job for this cluster. Currently, the only job type supported for clusters is <code>LOCAL_USE</code>.</p> <p>For more information, see \\\"https://docs.aws.amazon.com/snowball/latest/snowcone-guide/snow-device-types.html\\\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i> or \\\"https://docs.aws.amazon.com/snowball/latest/developer-guide/snow-device-types.html\\\" (Snow Family Devices and Capacity)\
  \ in the <i>Snowcone User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"Resources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobResource\"\n        },\n        {\n          \"description\": \"The resources associated with the cluster job. These resources include Amazon S3 buckets and optional Lambda functions written in the Python language. \"\n        }\n      ]\n    },\n    \"OnDeviceServiceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OnDeviceServiceConfiguration\"\n        },\n        {\n          \"description\": \"Specifies the service or services on the Snow Family device that your transferred data will be exported from or imported into. Amazon Web Services Snow Family device clusters support Amazon S3 and NFS (Network File System).\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n       \
  \ {\n          \"description\": \"An optional description of this specific cluster, for example <code>Environmental Data Cluster-01</code>.\"\n        }\n      ]\n    },\n    \"AddressId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressId\"\n        },\n        {\n          \"description\": \"The ID for the address that you want the cluster shipped to.\"\n        }\n      ]\n    },\n    \"KmsKeyARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyARN\"\n        },\n        {\n          \"description\": \"The <code>KmsKeyARN</code> value that you want to associate with this cluster. <code>KmsKeyARN</code> values are created by using the <a href=\\\"https://docs.aws.amazon.com/kms/latest/APIReference/API_CreateKey.html\\\">CreateKey</a> API action in Key Management Service (KMS). \"\n        }\n      ]\n    },\n    \"RoleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleARN\"\n\
  \        },\n        {\n          \"description\": \"The <code>RoleARN</code> that you want to associate with this cluster. <code>RoleArn</code> values are created by using the <a href=\\\"https://docs.aws.amazon.com/IAM/latest/APIReference/API_CreateRole.html\\\">CreateRole</a> API action in Identity and Access Management (IAM).\"\n        }\n      ]\n    },\n    \"SnowballType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnowballType\"\n        },\n        {\n          \"description\": \"<p>The type of Snow Family devices to use for this cluster. </p> <note> <p>For cluster jobs, Amazon Web Services Snow Family currently supports only the <code>EDGE</code> device type.</p> </note> <p>For more information, see \\\"https://docs.aws.amazon.com/snowball/latest/snowcone-guide/snow-device-types.html\\\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i> or \\\"https://docs.aws.amazon.com/snowball/latest/developer-guide/snow-device-types.html\\\
  \" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"ShippingOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShippingOption\"\n        },\n        {\n          \"description\": \"<p>The shipping speed for each node in this cluster. This speed doesn't dictate how soon you'll get each Snowball Edge device, rather it represents how quickly each device moves to its destination while in transit. Regional shipping speeds are as follows: </p> <ul> <li> <p>In Australia, you have access to express shipping. Typically, Snow devices shipped express are delivered in about a day.</p> </li> <li> <p>In the European Union (EU), you have access to express shipping. Typically, Snow devices shipped express are delivered in about a day. In addition, most countries in the EU have access to standard shipping, which typically takes less than a week, one way.</p> </li> <li> <p>In India, Snow devices are delivered\
  \ in one to seven days.</p> </li> <li> <p>In the United States of America (US), you have access to one-day shipping and two-day shipping.</p> </li> </ul> <ul> <li> <p>In Australia, you have access to express shipping. Typically, devices shipped express are delivered in about a day.</p> </li> <li> <p>In the European Union (EU), you have access to express shipping. Typically, Snow devices shipped express are delivered in about a day. In addition, most countries in the EU have access to standard shipping, which typically takes less than a week, one way.</p> </li> <li> <p>In India, Snow devices are delivered in one to seven days.</p> </li> <li> <p>In the US, you have access to one-day shipping and two-day shipping.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Notification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Notification\"\n        },\n        {\n          \"description\": \"The Amazon Simple Notification Service (Amazon SNS) notification\
  \ settings for this cluster.\"\n        }\n      ]\n    },\n    \"ForwardingAddressId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressId\"\n        },\n        {\n          \"description\": \"The forwarding address ID for a cluster. This field is not supported in most regions.\"\n        }\n      ]\n    },\n    \"TaxDocuments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaxDocuments\"\n        },\n        {\n          \"description\": \"The tax documents required in your Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"RemoteManagement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemoteManagement\"\n        },\n        {\n          \"description\": \"Allows you to securely operate and manage Snow devices in a cluster remotely from outside of your internal network. When set to <code>INSTALLED_AUTOSTART</code>, remote management will automatically be available when\
  \ the device arrives at your location. Otherwise, you need to use the Snowball Client to manage the device.\"\n        }\n      ]\n    },\n    \"InitialClusterSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InitialClusterSize\"\n        },\n        {\n          \"description\": \"If provided, each job will be automatically created and associated with the new cluster. If not provided, will be treated as 0.\"\n        }\n      ]\n    },\n    \"ForceCreateJobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"Force to create cluster when user attempts to overprovision or underprovision a cluster. A cluster is overprovisioned or underprovisioned if the initial size of the cluster is more (overprovisioned) or less (underprovisioned) than what needed to meet capacity requirement specified with <code>OnDeviceServiceConfiguration</code>.\"\n        }\n      ]\n    },\n\
  \    \"LongTermPricingIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongTermPricingIdList\"\n        },\n        {\n          \"description\": \"Lists long-term pricing id that will be used to associate with jobs automatically created for the new cluster.\"\n        }\n      ]\n    },\n    \"SnowballCapacityPreference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnowballCapacity\"\n        },\n        {\n          \"description\": \"<p>If your job is being created in one of the US regions, you have the option of specifying what size Snow device you'd like for this job. In all other regions, Snowballs come with 80 TB in storage capacity.</p> <p>For more information, see \\\"https://docs.aws.amazon.com/snowball/latest/snowcone-guide/snow-device-types.html\\\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i> or \\\"https://docs.aws.amazon.com/snowball/latest/developer-guide/snow-device-types.html\\\
  \" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobType\",\n    \"AddressId\",\n    \"SnowballType\",\n    \"ShippingOption\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-cluster-request-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: CreateClusterRequest
---
