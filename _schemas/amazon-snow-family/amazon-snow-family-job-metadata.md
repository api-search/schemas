---
description: Contains information about a specific job including shipping information, job status, and other important metadata. This information is returned as a part of the response syntax of the <code>DescribeJob</code> action.
layout: schema
name: JobMetadata
properties_list:
- description: ''
  name: JobId
  type: object
- description: ''
  name: JobState
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
  name: Description
  type: object
- description: ''
  name: KmsKeyARN
  type: object
- description: ''
  name: RoleARN
  type: object
- description: ''
  name: AddressId
  type: object
- description: ''
  name: ShippingDetails
  type: object
- description: ''
  name: SnowballCapacityPreference
  type: object
- description: ''
  name: Notification
  type: object
- description: ''
  name: DataTransferProgress
  type: object
- description: ''
  name: JobLogInfo
  type: object
- description: ''
  name: ClusterId
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
  name: OnDeviceServiceConfiguration
  type: object
- description: ''
  name: ImpactLevel
  type: object
- description: ''
  name: PickupDetails
  type: object
- description: ''
  name: SnowballId
  type: object
provider_name: Amazon Snow Family
provider_slug: amazon-snow-family
schema_file: json-schema/amazon-snow-family-job-metadata-schema.json
slug: amazon-snow-family-job-metadata
source_filename: amazon-snow-family-job-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-job-metadata-schema.json\",\n  \"title\": \"JobMetadata\",\n  \"description\": \"Contains information about a specific job including shipping information, job status, and other important metadata. This information is returned as a part of the response syntax of the <code>DescribeJob</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The automatically generated ID for a job, for example <code>JID123e4567-e89b-12d3-a456-426655440000</code>.\"\n        }\n      ]\n    },\n    \"JobState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobState\"\n        },\n        {\n          \"description\"\
  : \"The current status of the jobs.\"\n        }\n      ]\n    },\n    \"JobType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobType\"\n        },\n        {\n          \"description\": \"The type of job.\"\n        }\n      ]\n    },\n    \"SnowballType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnowballType\"\n        },\n        {\n          \"description\": \"The type of device used with this job.\"\n        }\n      ]\n    },\n    \"CreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The creation date for this job.\"\n        }\n      ]\n    },\n    \"Resources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobResource\"\n        },\n        {\n          \"description\": \"An array of <code>S3Resource</code> objects. Each <code>S3Resource</code> object represents an Amazon\
  \ S3 bucket that your transferred data will be exported from or imported into.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The description of the job, provided at job creation.\"\n        }\n      ]\n    },\n    \"KmsKeyARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KmsKeyARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) for the Key Management Service (KMS) key associated with this job. This ARN was created using the <a href=\\\"https://docs.aws.amazon.com/kms/latest/APIReference/API_CreateKey.html\\\">CreateKey</a> API action in KMS.\"\n        }\n      ]\n    },\n    \"RoleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleARN\"\n        },\n        {\n          \"description\": \"The role ARN associated with this job. This ARN\
  \ was created using the <a href=\\\"https://docs.aws.amazon.com/IAM/latest/APIReference/API_CreateRole.html\\\">CreateRole</a> API action in Identity and Access Management.\"\n        }\n      ]\n    },\n    \"AddressId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressId\"\n        },\n        {\n          \"description\": \"The ID for the address that you want the Snow device shipped to.\"\n        }\n      ]\n    },\n    \"ShippingDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ShippingDetails\"\n        },\n        {\n          \"description\": \"A job's shipping information, including inbound and outbound tracking numbers and shipping speed options.\"\n        }\n      ]\n    },\n    \"SnowballCapacityPreference\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnowballCapacity\"\n        },\n        {\n          \"description\": \"<p>The Snow device capacity preference for this\
  \ job, specified at job creation. In US regions, you can choose between 50 TB and 80 TB Snowballs. All other regions use 80 TB capacity Snowballs.</p> <p>For more information, see \\\"https://docs.aws.amazon.com/snowball/latest/snowcone-guide/snow-device-types.html\\\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i> or \\\"https://docs.aws.amazon.com/snowball/latest/developer-guide/snow-device-types.html\\\" (Snow Family Devices and Capacity) in the <i>Snowcone User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"Notification\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Notification\"\n        },\n        {\n          \"description\": \"The Amazon Simple Notification Service (Amazon SNS) notification settings associated with a specific job. The <code>Notification</code> object is returned as a part of the response syntax of the <code>DescribeJob</code> action in the <code>JobMetadata</code> data type.\"\n        }\n      ]\n \
  \   },\n    \"DataTransferProgress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataTransfer\"\n        },\n        {\n          \"description\": \"A value that defines the real-time status of a Snow device's data transfer while the device is at Amazon Web Services. This data is only available while a job has a <code>JobState</code> value of <code>InProgress</code>, for both import and export jobs.\"\n        }\n      ]\n    },\n    \"JobLogInfo\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobLogs\"\n        },\n        {\n          \"description\": \"Links to Amazon S3 presigned URLs for the job report and logs. For import jobs, the PDF job report becomes available at the end of the import process. For export jobs, your job report typically becomes available while the Snow device for your job part is being delivered to you.\"\n        }\n      ]\n    },\n    \"ClusterId\": {\n      \"allOf\": [\n        {\n        \
  \  \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The 39-character ID for the cluster, for example <code>CID123e4567-e89b-12d3-a456-426655440000</code>.\"\n        }\n      ]\n    },\n    \"ForwardingAddressId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AddressId\"\n        },\n        {\n          \"description\": \"The ID of the address that you want a job shipped to, after it will be shipped to its primary address. This field is not supported in most regions.\"\n        }\n      ]\n    },\n    \"TaxDocuments\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TaxDocuments\"\n        },\n        {\n          \"description\": \"The metadata associated with the tax documents required in your Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"DeviceConfiguration\": {\n      \"$ref\": \"#/components/schemas/DeviceConfiguration\"\n    },\n    \"RemoteManagement\":\
  \ {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RemoteManagement\"\n        },\n        {\n          \"description\": \"Allows you to securely operate and manage Snowcone devices remotely from outside of your internal network. When set to <code>INSTALLED_AUTOSTART</code>, remote management will automatically be available when the device arrives at your location. Otherwise, you need to use the Snowball Client to manage the device.\"\n        }\n      ]\n    },\n    \"LongTermPricingId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LongTermPricingId\"\n        },\n        {\n          \"description\": \"The ID of the long-term pricing type for the device.\"\n        }\n      ]\n    },\n    \"OnDeviceServiceConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OnDeviceServiceConfiguration\"\n        },\n        {\n          \"description\": \"Represents metadata and configuration settings\
  \ for services on an Amazon Web Services Snow Family device.\"\n        }\n      ]\n    },\n    \"ImpactLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ImpactLevel\"\n        },\n        {\n          \"description\": \"The highest impact level of data that will be stored or processed on the device, provided at job creation.\"\n        }\n      ]\n    },\n    \"PickupDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PickupDetails\"\n        },\n        {\n          \"description\": \"Information identifying the person picking up the device.\"\n        }\n      ]\n    },\n    \"SnowballId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Unique ID associated with a device.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-snow-family/refs/heads/main/json-schema/amazon-snow-family-job-metadata-schema.json
tags:
- AWS
- Data Migration
- Edge Computing
- Offline Transfer
- Physical Appliance
title: JobMetadata
---
