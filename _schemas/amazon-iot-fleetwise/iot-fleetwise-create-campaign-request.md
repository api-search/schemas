---
description: CreateCampaignRequest schema
layout: schema
name: CreateCampaignRequest
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: description
  type: object
- description: ''
  name: signalCatalogArn
  type: object
- description: ''
  name: targetArn
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: expiryTime
  type: object
- description: ''
  name: postTriggerCollectionDuration
  type: object
- description: ''
  name: diagnosticsMode
  type: object
- description: ''
  name: spoolingMode
  type: object
- description: ''
  name: compression
  type: object
- description: ''
  name: priority
  type: object
- description: ''
  name: signalsToCollect
  type: object
- description: ''
  name: collectionScheme
  type: object
- description: ''
  name: dataExtraDimensions
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: dataDestinationConfigs
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-create-campaign-request-schema.json
slug: iot-fleetwise-create-campaign-request
source_filename: iot-fleetwise-create-campaign-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-campaign-request-schema.json\",\n  \"title\": \"CreateCampaignRequest\",\n  \"description\": \"CreateCampaignRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/campaignName\"\n        },\n        {\n          \"description\": \" The name of the campaign to create. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \"An optional description of the campaign to help identify its purpose.\"\n        }\n      ]\n    },\n    \"signalCatalogArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n\
  \        {\n          \"description\": \"(Optional) The Amazon Resource Name (ARN) of the signal catalog to associate with the campaign. \"\n        }\n      ]\n    },\n    \"targetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \" The ARN of the vehicle or fleet to deploy a campaign to. \"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \"<p>(Optional) The time, in milliseconds, to deliver a campaign after it was approved. If it's not specified, <code>0</code> is used.</p> <p>Default: <code>0</code> </p>\"\n        }\n      ]\n    },\n    \"expiryTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \"<p> (Optional) The time the campaign expires, in seconds since\
  \ epoch (January 1, 1970 at midnight UTC time). Vehicle data isn't collected after the campaign expires. </p> <p>Default: 253402214400 (December 31, 9999, 00:00:00 UTC)</p>\"\n        }\n      ]\n    },\n    \"postTriggerCollectionDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/uint32\"\n        },\n        {\n          \"description\": \"<p> (Optional) How long (in milliseconds) to collect raw data after a triggering event initiates the collection. If it's not specified, <code>0</code> is used.</p> <p>Default: <code>0</code> </p>\"\n        }\n      ]\n    },\n    \"diagnosticsMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DiagnosticsMode\"\n        },\n        {\n          \"description\": \"<p> (Optional) Option for a vehicle to send diagnostic trouble codes to Amazon Web Services IoT FleetWise. If you want to send diagnostic trouble codes, use <code>SEND_ACTIVE_DTCS</code>. If it's not specified, <code>OFF</code>\
  \ is used.</p> <p>Default: <code>OFF</code> </p>\"\n        }\n      ]\n    },\n    \"spoolingMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpoolingMode\"\n        },\n        {\n          \"description\": \"<p>(Optional) Whether to store collected data after a vehicle lost a connection with the cloud. After a connection is re-established, the data is automatically forwarded to Amazon Web Services IoT FleetWise. If you want to store collected data when a vehicle loses connection with the cloud, use <code>TO_DISK</code>. If it's not specified, <code>OFF</code> is used.</p> <p>Default: <code>OFF</code> </p>\"\n        }\n      ]\n    },\n    \"compression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Compression\"\n        },\n        {\n          \"description\": \"<p> (Optional) Whether to compress signals before transmitting data to Amazon Web Services IoT FleetWise. If you don't want to compress the signals, use\
  \ <code>OFF</code>. If it's not specified, <code>SNAPPY</code> is used. </p> <p>Default: <code>SNAPPY</code> </p>\"\n        }\n      ]\n    },\n    \"priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/priority\"\n        },\n        {\n          \"description\": \"<p>(Optional) A number indicating the priority of one campaign over another campaign for a certain vehicle or fleet. A campaign with the lowest value is deployed to vehicles before any other campaigns. If it's not specified, <code>0</code> is used. </p> <p>Default: <code>0</code> </p>\"\n        }\n      ]\n    },\n    \"signalsToCollect\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SignalInformationList\"\n        },\n        {\n          \"description\": \"(Optional) A list of information about signals to collect. \"\n        }\n      ]\n    },\n    \"collectionScheme\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CollectionScheme\"\
  \n        },\n        {\n          \"description\": \" The data collection scheme associated with the campaign. You can specify a scheme that collects data based on time or an event.\"\n        }\n      ]\n    },\n    \"dataExtraDimensions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataExtraDimensionNodePathList\"\n        },\n        {\n          \"description\": \"<p> (Optional) A list of vehicle attributes to associate with a campaign. </p> <p>Enrich the data with specified vehicle attributes. For example, add <code>make</code> and <code>model</code> to the campaign, and Amazon Web Services IoT FleetWise will associate the data with those attributes as dimensions in Amazon Timestream. You can then query the data against <code>make</code> and <code>model</code>.</p> <p>Default: An empty array</p>\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n       \
  \ {\n          \"description\": \"Metadata that can be used to manage the campaign.\"\n        }\n      ]\n    },\n    \"dataDestinationConfigs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataDestinationConfigs\"\n        },\n        {\n          \"description\": \"<p>The destination where the campaign sends data. You can choose to send data to be stored in Amazon S3 or Amazon Timestream.</p> <p>Amazon S3 optimizes the cost of data storage and provides additional mechanisms to use vehicle data, such as data lakes, centralized data storage, data processing pipelines, and analytics. </p> <p>You can use Amazon Timestream to access and analyze time series data, and Timestream to query vehicle data so that you can identify trends and patterns.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"signalCatalogArn\",\n    \"targetArn\",\n    \"collectionScheme\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-create-campaign-request-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: CreateCampaignRequest
---
