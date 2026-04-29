---
description: CreateJobRequest schema from Amazon Snow Family API
layout: schema
name: CreateJobRequest
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
  name: SnowballCapacityPreference
  type: object
- description: ''
  name: ShippingOption
  type: object
- description: ''
  name: Notification
  type: object
- description: ''
  name: ClusterId
  type: object
- description: ''
  name: SnowballType
  type: object
- description: ''
  name: ForwardingAddressId
  type: object
- description: ''
  name: TaxDocuments
  type: object
- description: ''
  name: DeviceConfiguration
  type: object
- description: ''
  name: RemoteManagement
  type: object
- description: ''
  name: LongTermPricingId
  type: object
- description: ''
  name: ImpactLevel
  type: object
- description: ''
  name: PickupDetails
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-create-job-request-schema.json
slug: amazon-snow-family-create-job-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-job-request-schema.json\",\n  \"title\": \"CreateJobRequest\",\n  \"description\": \"CreateJobRequest schema from Amazon Snow Family API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobType\"\n        },\n        {\n          \"description\": \"Defines the type of job that you're creating. \"\n        }\n      ]\n    },\n    \"Resources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobResource\"\n        },\n        {\n          \"description\": \"<p>Defines the Amazon S3 buckets associated with this job.</p> <p>With <code>IMPORT</code> jobs, you specify the bucket or buckets that your transferred data will be imported into.</p> <p>With <code>EXPORT</code>\
  \ jobs, you specify the bucket or buckets that your transferred data will be exported from. Optionally, you can also specify a <code>KeyRange</code> value. If you choose to export a range, you define the length of the range by providing either an inclusive <code>BeginMarker</code> value, an inclusive <code>EndMarker</code> value, or both. Ranges are UTF-8 binary sorted.</p>\"\n        }\n      ]\n    },\n    \"OnDeviceServiceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OnDeviceServiceConfiguration\"\n        },\n        {\n          \"description\": \"Specifies the service or services on the Snow Family device that your transferred data will be exported from or imported into. Amazon Web Services Snow Family supports Amazon S3 and NFS (Network File System) and the Amazon Web Services Storage Gateway service Tape Gateway type.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\
  \n        },\n        {\n          \"description\": \"Defines an optional description of this specific job, for example <code>Important Photos 2016-08-11</code>.\"\n        }\n      ]\n    },\n    \"AddressId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressId\"\n        },\n        {\n          \"description\": \"The ID for the address that you want the Snow device shipped to.\"\n        }\n      ]\n    },\n    \"KmsKeyARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyARN\"\n        },\n        {\n          \"description\": \"The <code>KmsKeyARN</code> that you want to associate with this job. <code>KmsKeyARN</code>s are created using the <a href=\\\"https://docs.aws.amazon.com/kms/latest/APIReference/API_CreateKey.html\\\">CreateKey</a> Key Management Service (KMS) API action.\"\n        }\n      ]\n    },\n    \"RoleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleARN\"\
  \n        },\n        {\n          \"description\": \"The <code>RoleARN</code> that you want to associate with this job. <code>RoleArn</code>s are created using the <a href=\\\"https://docs.aws.amazon.com/IAM/latest/APIReference/API_CreateRole.html\\\">CreateRole</a> Identity and Access Management (IAM) API action.\"\n        }\n      ]\n    },\n    \"SnowballCapacityPreference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnowballCapacity\"\n        },\n        {\n          \"description\": \"<p>If your job is being created in one of the US regions, you have the option of specifying what size Snow device you'd like for this job. In all other regions, Snowballs come with 80 TB in storage capacity.</p> <p>For more information, see \\\"https://docs.aws.amazon.com/snowball/latest/snowcone-guide/snow-device-types.html\\\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i> or \\\"https://docs.aws.amazon.com/snowball/latest/developer-guide/snow-device-types.html\\\
  \" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"ShippingOption\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShippingOption\"\n        },\n        {\n          \"description\": \"<p>The shipping speed for this job. This speed doesn't dictate how soon you'll get the Snow device, rather it represents how quickly the Snow device moves to its destination while in transit. Regional shipping speeds are as follows:</p> <ul> <li> <p>In Australia, you have access to express shipping. Typically, Snow devices shipped express are delivered in about a day.</p> </li> <li> <p>In the European Union (EU), you have access to express shipping. Typically, Snow devices shipped express are delivered in about a day. In addition, most countries in the EU have access to standard shipping, which typically takes less than a week, one way.</p> </li> <li> <p>In India, Snow devices are delivered in one to seven days.</p>\
  \ </li> <li> <p>In the US, you have access to one-day shipping and two-day shipping.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Notification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Notification\"\n        },\n        {\n          \"description\": \"Defines the Amazon Simple Notification Service (Amazon SNS) notification settings for this job.\"\n        }\n      ]\n    },\n    \"ClusterId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ClusterId\"\n        },\n        {\n          \"description\": \"The ID of a cluster. If you're creating a job for a node in a cluster, you need to provide only this <code>clusterId</code> value. The other job attributes are inherited from the cluster.\"\n        }\n      ]\n    },\n    \"SnowballType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnowballType\"\n        },\n        {\n          \"description\": \"<p>The type of Snow Family\
  \ devices to use for this job. </p> <note> <p>For cluster jobs, Amazon Web Services Snow Family currently supports only the <code>EDGE</code> device type.</p> </note> <p>The type of Amazon Web Services Snow device to use for this job. Currently, the only supported device type for cluster jobs is <code>EDGE</code>.</p> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/snowball/latest/developer-guide/device-differences.html\\\">Snowball Edge Device Options</a> in the Snowball Edge Developer Guide.</p> <p>For more information, see \\\"https://docs.aws.amazon.com/snowball/latest/snowcone-guide/snow-device-types.html\\\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i> or \\\"https://docs.aws.amazon.com/snowball/latest/developer-guide/snow-device-types.html\\\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"ForwardingAddressId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressId\"\
  \n        },\n        {\n          \"description\": \"The forwarding address ID for a job. This field is not supported in most Regions.\"\n        }\n      ]\n    },\n    \"TaxDocuments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaxDocuments\"\n        },\n        {\n          \"description\": \"The tax documents required in your Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"DeviceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeviceConfiguration\"\n        },\n        {\n          \"description\": \"<p>Defines the device configuration for an Snowcone job.</p> <p>For more information, see \\\"https://docs.aws.amazon.com/snowball/latest/snowcone-guide/snow-device-types.html\\\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i> or \\\"https://docs.aws.amazon.com/snowball/latest/developer-guide/snow-device-types.html\\\" (Snow Family Devices and Capacity) in the <i>Snowcone\
  \ User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"RemoteManagement\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemoteManagement\"\n        },\n        {\n          \"description\": \"Allows you to securely operate and manage Snowcone devices remotely from outside of your internal network. When set to <code>INSTALLED_AUTOSTART</code>, remote management will automatically be available when the device arrives at your location. Otherwise, you need to use the Snowball Edge client to manage the device. When set to <code>NOT_INSTALLED</code>, remote management will not be available on the device. \"\n        }\n      ]\n    },\n    \"LongTermPricingId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongTermPricingId\"\n        },\n        {\n          \"description\": \"The ID of the long-term pricing type for the device.\"\n        }\n      ]\n    },\n    \"ImpactLevel\": {\n      \"allOf\": [\n        {\n         \
  \ \"$ref\": \"#/components/schemas/ImpactLevel\"\n        },\n        {\n          \"description\": \"The highest impact level of data that will be stored or processed on the device, provided at job creation.\"\n        }\n      ]\n    },\n    \"PickupDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PickupDetails\"\n        },\n        {\n          \"description\": \"Information identifying the person picking up the device.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-create-job-request-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: CreateJobRequest
---
