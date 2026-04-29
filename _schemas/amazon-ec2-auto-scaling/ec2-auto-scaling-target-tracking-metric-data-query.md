---
description: The metric data to return. Also defines whether this call is returning data for one metric only, or whether it is performing a math expression on the values of returned metric statistics to create a new time series. A time series is a series of data points, each of which is associated with a timestamp.
layout: schema
name: TargetTrackingMetricDataQuery
properties_list:
- description: ''
  name: Id
  type: object
- description: ''
  name: Expression
  type: object
- description: ''
  name: MetricStat
  type: object
- description: ''
  name: Label
  type: object
- description: ''
  name: ReturnData
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-target-tracking-metric-data-query-schema.json
slug: ec2-auto-scaling-target-tracking-metric-data-query
source_filename: ec2-auto-scaling-target-tracking-metric-data-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-target-tracking-metric-data-query-schema.json\",\n  \"title\": \"TargetTrackingMetricDataQuery\",\n  \"description\": \"The metric data to return. Also defines whether this call is returning data for one metric only, or whether it is performing a math expression on the values of returned metric statistics to create a new time series. A time series is a series of data points, each of which is associated with a timestamp.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"A short name that identifies the object's results in the response. This name must be unique among all <code>TargetTrackingMetricDataQuery</code> objects\
  \ specified for a single scaling policy. If you are performing math expressions on this set of data, this name represents that data and can serve as a variable in the mathematical expression. The valid characters are letters, numbers, and underscores. The first character must be a lowercase letter. \"\n        }\n      ]\n    },\n    \"Expression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen2047\"\n        },\n        {\n          \"description\": \"<p>The math expression to perform on the returned data, if this object is performing a math expression. This expression can use the <code>Id</code> of the other metrics to refer to those metrics, and can also use the <code>Id</code> of other expressions to use the result of those expressions. </p> <p>Conditional: Within each <code>TargetTrackingMetricDataQuery</code> object, you must specify either <code>Expression</code> or <code>MetricStat</code>, but not both.</p>\"\n        }\n      ]\n\
  \    },\n    \"MetricStat\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetTrackingMetricStat\"\n        },\n        {\n          \"description\": \"<p>Information about the metric data to return.</p> <p>Conditional: Within each <code>TargetTrackingMetricDataQuery</code> object, you must specify either <code>Expression</code> or <code>MetricStat</code>, but not both.</p>\"\n        }\n      ]\n    },\n    \"Label\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMetricLabel\"\n        },\n        {\n          \"description\": \"A human-readable label for this metric or expression. This is especially useful if this is a math expression, so that you know what the value represents.\"\n        }\n      ]\n    },\n    \"ReturnData\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReturnData\"\n        },\n        {\n          \"description\": \"<p>Indicates whether to return the timestamps\
  \ and raw data values of this metric. </p> <p>If you use any math expressions, specify <code>true</code> for this value for only the final math expression that the metric specification is based on. You must specify <code>false</code> for <code>ReturnData</code> for all the other metrics and expressions used in the metric specification.</p> <p>If you are only retrieving metrics and not performing any math expressions, do not specify anything for <code>ReturnData</code>. This sets it to its default (<code>true</code>).</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-target-tracking-metric-data-query-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- AWS
- Compute
- EC2
- High Availability
- Scaling
title: TargetTrackingMetricDataQuery
---
