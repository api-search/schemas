---
description: DescribeTimeSeriesResponse schema
layout: schema
name: DescribeTimeSeriesResponse
properties_list:
- description: ''
  name: assetId
  type: object
- description: ''
  name: propertyId
  type: object
- description: ''
  name: alias
  type: object
- description: ''
  name: timeSeriesId
  type: object
- description: ''
  name: dataType
  type: object
- description: ''
  name: dataTypeSpec
  type: object
- description: ''
  name: timeSeriesCreationDate
  type: object
- description: ''
  name: timeSeriesLastUpdateDate
  type: object
- description: ''
  name: timeSeriesArn
  type: object
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
schema_file: json-schema/iot-sitewise-describe-time-series-response-schema.json
slug: iot-sitewise-describe-time-series-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-time-series-response-schema.json\",\n  \"title\": \"DescribeTimeSeriesResponse\",\n  \"description\": \"DescribeTimeSeriesResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the asset in which the asset property was created.\"\n        }\n      ]\n    },\n    \"propertyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ID\"\n        },\n        {\n          \"description\": \"The ID of the asset property.\"\n        }\n      ]\n    },\n    \"alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyAlias\"\n        },\n        {\n      \
  \    \"description\": \"The alias that identifies the time series.\"\n        }\n      ]\n    },\n    \"timeSeriesId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeSeriesId\"\n        },\n        {\n          \"description\": \"The ID of the time series.\"\n        }\n      ]\n    },\n    \"dataType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PropertyDataType\"\n        },\n        {\n          \"description\": \"<p>The data type of the time series.</p> <p>If you specify <code>STRUCT</code>, you must also specify <code>dataTypeSpec</code> to identify the type of the structure for this time series.</p>\"\n        }\n      ]\n    },\n    \"dataTypeSpec\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Name\"\n        },\n        {\n          \"description\": \"<p>The data type of the structure for this time series. This parameter is required for time series that have the <code>STRUCT</code>\
  \ data type.</p> <p>The options for this parameter depend on the type of the composite model in which you created the asset property that is associated with your time series. Use <code>AWS/ALARM_STATE</code> for alarm state in alarm composite models.</p>\"\n        }\n      ]\n    },\n    \"timeSeriesCreationDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date that the time series was created, in Unix epoch time.\"\n        }\n      ]\n    },\n    \"timeSeriesLastUpdateDate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date that the time series was last updated, in Unix epoch time.\"\n        }\n      ]\n    },\n    \"timeSeriesArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ARN\"\n        },\n        {\n          \"description\": \"<p>The <a href=\\\
  \"https://docs.aws.amazon.com/general/latest/gr/aws-arns-and-namespaces.html\\\">ARN</a> of the time series, which has the following format.</p> <p> <code>arn:${Partition}:iotsitewise:${Region}:${Account}:time-series/${TimeSeriesId}</code> </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"timeSeriesId\",\n    \"dataType\",\n    \"timeSeriesCreationDate\",\n    \"timeSeriesLastUpdateDate\",\n    \"timeSeriesArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/json-schema/iot-sitewise-describe-time-series-response-schema.json
tags:
- AWS
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
title: DescribeTimeSeriesResponse
---
