---
description: PutStorageConfigurationResponse schema
layout: schema
name: PutStorageConfigurationResponse
properties_list:
- description: ''
  name: storageType
  type: object
- description: ''
  name: multiLayerStorage
  type: object
- description: ''
  name: disassociatedDataStorage
  type: object
- description: How many days your data is kept in the hot tier. By default, your data is kept indefinitely in the hot tier.
  name: retentionPeriod
  type: object
- description: Contains current status information for the configuration.
  name: configurationStatus
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-put-storage-configuration-response-schema.json
slug: iot-sitewise-put-storage-configuration-response
source_filename: iot-sitewise-put-storage-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-put-storage-configuration-response-schema.json\",\n  \"title\": \"PutStorageConfigurationResponse\",\n  \"description\": \"PutStorageConfigurationResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"storageType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StorageType\"\n        },\n        {\n          \"description\": \"<p>The storage tier that you specified for your data. The <code>storageType</code> parameter can be one of the following values:</p> <ul> <li> <p> <code>SITEWISE_DEFAULT_STORAGE</code> \\u2013 IoT SiteWise saves your data into the hot tier. The hot tier is a service-managed database.</p> </li> <li> <p> <code>MULTI_LAYER_STORAGE</code> \\u2013 IoT SiteWise saves your data in both the cold tier and the hot tier. The cold\
  \ tier is a customer-managed Amazon S3 bucket.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"multiLayerStorage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MultiLayerStorage\"\n        },\n        {\n          \"description\": \"Contains information about the storage destination.\"\n        }\n      ]\n    },\n    \"disassociatedDataStorage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisassociatedDataStorageState\"\n        },\n        {\n          \"description\": \"<p>Contains the storage configuration for time series (data streams) that aren't associated with asset properties. The <code>disassociatedDataStorage</code> can be one of the following values:</p> <ul> <li> <p> <code>ENABLED</code> \\u2013 IoT SiteWise accepts time series that aren't associated with asset properties.</p> <important> <p>After the <code>disassociatedDataStorage</code> is enabled, you can't disable it.</p> </important> </li> <li> <p>\
  \ <code>DISABLED</code> \\u2013 IoT SiteWise doesn't accept time series (data streams) that aren't associated with asset properties.</p> </li> </ul> <p>For more information, see <a href=\\\"https://docs.aws.amazon.com/iot-sitewise/latest/userguide/data-streams.html\\\">Data streams</a> in the <i>IoT SiteWise User Guide</i>.</p>\"\n        }\n      ]\n    },\n    \"retentionPeriod\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"numberOfDays\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/NumberOfDays\"\n            },\n            {\n              \"description\": \"<p>The number of days that your data is kept.</p> <note> <p>If you specified a value for this parameter, the <code>unlimited</code> parameter must be <code>false</code>.</p> </note>\"\n            }\n          ]\n        },\n        \"unlimited\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/Unlimited\"\n           \
  \ },\n            {\n              \"description\": \"<p>If true, your data is kept indefinitely.</p> <note> <p>If configured to <code>true</code>, you must not specify a value for the <code>numberOfDays</code> parameter.</p> </note>\"\n            }\n          ]\n        }\n      },\n      \"description\": \"How many days your data is kept in the hot tier. By default, your data is kept indefinitely in the hot tier.\"\n    },\n    \"configurationStatus\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"state\"\n      ],\n      \"properties\": {\n        \"state\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ConfigurationState\"\n            },\n            {\n              \"description\": \"The current state of the configuration.\"\n            }\n          ]\n        },\n        \"error\": {\n          \"allOf\": [\n            {\n              \"$ref\": \"#/components/schemas/ConfigurationErrorDetails\"\n            },\n\
  \            {\n              \"description\": \"Contains associated error information, if any.\"\n            }\n          ]\n        }\n      },\n      \"description\": \"Contains current status information for the configuration.\"\n    }\n  },\n  \"required\": [\n    \"storageType\",\n    \"configurationStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-put-storage-configuration-response-schema.json
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: PutStorageConfigurationResponse
---
