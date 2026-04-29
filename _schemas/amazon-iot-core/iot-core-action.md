---
description: Describes the actions associated with a rule.
layout: schema
name: Action
properties_list:
- description: ''
  name: dynamoDB
  type: object
- description: ''
  name: dynamoDBv2
  type: object
- description: ''
  name: lambda
  type: object
- description: ''
  name: sns
  type: object
- description: ''
  name: sqs
  type: object
- description: ''
  name: kinesis
  type: object
- description: ''
  name: republish
  type: object
- description: ''
  name: s3
  type: object
- description: ''
  name: firehose
  type: object
- description: ''
  name: cloudwatchMetric
  type: object
- description: ''
  name: cloudwatchAlarm
  type: object
- description: ''
  name: cloudwatchLogs
  type: object
- description: ''
  name: elasticsearch
  type: object
- description: ''
  name: salesforce
  type: object
- description: ''
  name: iotAnalytics
  type: object
- description: ''
  name: iotEvents
  type: object
- description: ''
  name: iotSiteWise
  type: object
- description: ''
  name: stepFunctions
  type: object
- description: ''
  name: timestream
  type: object
- description: ''
  name: http
  type: object
- description: ''
  name: kafka
  type: object
- description: ''
  name: openSearch
  type: object
- description: ''
  name: location
  type: object
provider_name: Amazon IoT Core
provider_slug: amazon-iot-core
schema_file: json-schema/iot-core-action-schema.json
slug: iot-core-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-action-schema.json\",\n  \"title\": \"Action\",\n  \"description\": \"Describes the actions associated with a rule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dynamoDB\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DynamoDBAction\"\n        },\n        {\n          \"description\": \"Write to a DynamoDB table.\"\n        }\n      ]\n    },\n    \"dynamoDBv2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DynamoDBv2Action\"\n        },\n        {\n          \"description\": \"Write to a DynamoDB table. This is a new version of the DynamoDB action. It allows you to write each attribute in an MQTT message payload into a separate DynamoDB column.\"\n        }\n      ]\n    },\n    \"lambda\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/LambdaAction\"\n        },\n        {\n          \"description\": \"Invoke a Lambda function.\"\n        }\n      ]\n    },\n    \"sns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnsAction\"\n        },\n        {\n          \"description\": \"Publish to an Amazon SNS topic.\"\n        }\n      ]\n    },\n    \"sqs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SqsAction\"\n        },\n        {\n          \"description\": \"Publish to an Amazon SQS queue.\"\n        }\n      ]\n    },\n    \"kinesis\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisAction\"\n        },\n        {\n          \"description\": \"Write data to an Amazon Kinesis stream.\"\n        }\n      ]\n    },\n    \"republish\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RepublishAction\"\n        },\n        {\n          \"description\"\
  : \"Publish to another MQTT topic.\"\n        }\n      ]\n    },\n    \"s3\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Action\"\n        },\n        {\n          \"description\": \"Write to an Amazon S3 bucket.\"\n        }\n      ]\n    },\n    \"firehose\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FirehoseAction\"\n        },\n        {\n          \"description\": \"Write to an Amazon Kinesis Firehose stream.\"\n        }\n      ]\n    },\n    \"cloudwatchMetric\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudwatchMetricAction\"\n        },\n        {\n          \"description\": \"Capture a CloudWatch metric.\"\n        }\n      ]\n    },\n    \"cloudwatchAlarm\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudwatchAlarmAction\"\n        },\n        {\n          \"description\": \"Change the state of a CloudWatch alarm.\"\n        }\n     \
  \ ]\n    },\n    \"cloudwatchLogs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CloudwatchLogsAction\"\n        },\n        {\n          \"description\": \"Send data to CloudWatch Logs.\"\n        }\n      ]\n    },\n    \"elasticsearch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ElasticsearchAction\"\n        },\n        {\n          \"description\": \"<p>Write data to an Amazon OpenSearch Service domain.</p> <note> <p>The <code>Elasticsearch</code> action can only be used by existing rule actions. To create a new rule action or to update an existing rule action, use the <code>OpenSearch</code> rule action instead. For more information, see <a href=\\\"https://docs.aws.amazon.com/iot/latest/apireference/API_OpenSearchAction.html\\\">OpenSearchAction</a>.</p> </note>\"\n        }\n      ]\n    },\n    \"salesforce\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SalesforceAction\"\n   \
  \     },\n        {\n          \"description\": \"Send a message to a Salesforce IoT Cloud Input Stream.\"\n        }\n      ]\n    },\n    \"iotAnalytics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IotAnalyticsAction\"\n        },\n        {\n          \"description\": \"Sends message data to an IoT Analytics channel.\"\n        }\n      ]\n    },\n    \"iotEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IotEventsAction\"\n        },\n        {\n          \"description\": \"Sends an input to an IoT Events detector.\"\n        }\n      ]\n    },\n    \"iotSiteWise\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IotSiteWiseAction\"\n        },\n        {\n          \"description\": \"Sends data from the MQTT message that triggered the rule to IoT SiteWise asset properties.\"\n        }\n      ]\n    },\n    \"stepFunctions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"\
  #/components/schemas/StepFunctionsAction\"\n        },\n        {\n          \"description\": \"Starts execution of a Step Functions state machine.\"\n        }\n      ]\n    },\n    \"timestream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestreamAction\"\n        },\n        {\n          \"description\": \"The Timestream rule action writes attributes (measures) from an MQTT message into an Amazon Timestream table. For more information, see the <a href=\\\"https://docs.aws.amazon.com/iot/latest/developerguide/timestream-rule-action.html\\\">Timestream</a> topic rule action documentation.\"\n        }\n      ]\n    },\n    \"http\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HttpAction\"\n        },\n        {\n          \"description\": \"Send data to an HTTPS endpoint.\"\n        }\n      ]\n    },\n    \"kafka\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KafkaAction\"\n       \
  \ },\n        {\n          \"description\": \"Send messages to an Amazon Managed Streaming for Apache Kafka (Amazon MSK) or self-managed Apache Kafka cluster.\"\n        }\n      ]\n    },\n    \"openSearch\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OpenSearchAction\"\n        },\n        {\n          \"description\": \"Write data to an Amazon OpenSearch Service domain.\"\n        }\n      ]\n    },\n    \"location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationAction\"\n        },\n        {\n          \"description\": \"The Amazon Location Service rule action sends device location updates from an MQTT message to an Amazon Location tracker resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-core/refs/heads/main/json-schema/iot-core-action-schema.json
tags:
- AWS
- Device Management
- IoT
- MQTT
- Message Routing
title: Action
---
