---
description: GetCampaignResponse schema
layout: schema
name: GetCampaignResponse
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: arn
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
  name: status
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
  name: creationTime
  type: object
- description: ''
  name: lastModificationTime
  type: object
- description: ''
  name: dataDestinationConfigs
  type: object
provider_name: Amazon IoT FleetWise
provider_slug: amazon-iot-fleetwise
schema_file: json-schema/iot-fleetwise-get-campaign-response-schema.json
slug: iot-fleetwise-get-campaign-response
source_filename: iot-fleetwise-get-campaign-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-campaign-response-schema.json\",\n  \"title\": \"GetCampaignResponse\",\n  \"description\": \"GetCampaignResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/campaignName\"\n        },\n        {\n          \"description\": \"The name of the campaign.\"\n        }\n      ]\n    },\n    \"arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the campaign. \"\n        }\n      ]\n    },\n    \"description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/description\"\n        },\n        {\n          \"description\": \"The description\
  \ of the campaign.\"\n        }\n      ]\n    },\n    \"signalCatalogArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \" The ARN of a signal catalog. \"\n        }\n      ]\n    },\n    \"targetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/arn\"\n        },\n        {\n          \"description\": \" The ARN of the vehicle or the fleet targeted by the campaign. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CampaignStatus\"\n        },\n        {\n          \"description\": \"The state of the campaign. The status can be one of: <code>CREATING</code>, <code>WAITING_FOR_APPROVAL</code>, <code>RUNNING</code>, and <code>SUSPENDED</code>. \"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n\
  \        {\n          \"description\": \" The time, in milliseconds, to deliver a campaign after it was approved.\"\n        }\n      ]\n    },\n    \"expiryTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \" The time the campaign expires, in seconds since epoch (January 1, 1970 at midnight UTC time). Vehicle data won't be collected after the campaign expires.\"\n        }\n      ]\n    },\n    \"postTriggerCollectionDuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/uint32\"\n        },\n        {\n          \"description\": \" How long (in seconds) to collect raw data after a triggering event initiates the collection. \"\n        }\n      ]\n    },\n    \"diagnosticsMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DiagnosticsMode\"\n        },\n        {\n          \"description\": \" Option for a vehicle to send\
  \ diagnostic trouble codes to Amazon Web Services IoT FleetWise. \"\n        }\n      ]\n    },\n    \"spoolingMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SpoolingMode\"\n        },\n        {\n          \"description\": \" Whether to store collected data after a vehicle lost a connection with the cloud. After a connection is re-established, the data is automatically forwarded to Amazon Web Services IoT FleetWise. \"\n        }\n      ]\n    },\n    \"compression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Compression\"\n        },\n        {\n          \"description\": \" Whether to compress signals before transmitting data to Amazon Web Services IoT FleetWise. If <code>OFF</code> is specified, the signals aren't compressed. If it's not specified, <code>SNAPPY</code> is used. \"\n        }\n      ]\n    },\n    \"priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/priority\"\
  \n        },\n        {\n          \"description\": \" A number indicating the priority of one campaign over another campaign for a certain vehicle or fleet. A campaign with the lowest value is deployed to vehicles before any other campaigns.\"\n        }\n      ]\n    },\n    \"signalsToCollect\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SignalInformationList\"\n        },\n        {\n          \"description\": \" Information about a list of signals to collect data on. \"\n        }\n      ]\n    },\n    \"collectionScheme\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CollectionScheme\"\n        },\n        {\n          \"description\": \" Information about the data collection scheme associated with the campaign. \"\n        }\n      ]\n    },\n    \"dataExtraDimensions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataExtraDimensionNodePathList\"\n        },\n        {\n          \"\
  description\": \" A list of vehicle attributes associated with the campaign. \"\n        }\n      ]\n    },\n    \"creationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \" The time the campaign was created in seconds since epoch (January 1, 1970 at midnight UTC time). \"\n        }\n      ]\n    },\n    \"lastModificationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/timestamp\"\n        },\n        {\n          \"description\": \"The last time the campaign was modified.\"\n        }\n      ]\n    },\n    \"dataDestinationConfigs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataDestinationConfigs\"\n        },\n        {\n          \"description\": \"<p>The destination where the campaign sends data. You can choose to send data to be stored in Amazon S3 or Amazon Timestream.</p> <p>Amazon S3 optimizes the cost of data\
  \ storage and provides additional mechanisms to use vehicle data, such as data lakes, centralized data storage, data processing pipelines, and analytics. </p> <p>You can use Amazon Timestream to access and analyze time series data, and Timestream to query vehicle data so that you can identify trends and patterns.</p>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-fleetwise/refs/heads/main/json-schema/iot-fleetwise-get-campaign-response-schema.json
tags:
- Automotive
- AWS
- Connected Vehicles
- IoT
- Telematics
- Vehicle Data
title: GetCampaignResponse
---
