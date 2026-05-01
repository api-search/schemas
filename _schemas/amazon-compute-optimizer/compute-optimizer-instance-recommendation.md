---
description: Describes an Amazon EC2 instance recommendation.
layout: schema
name: InstanceRecommendation
properties_list:
- description: ''
  name: instanceArn
  type: object
- description: ''
  name: accountId
  type: object
- description: ''
  name: instanceName
  type: object
- description: ''
  name: currentInstanceType
  type: object
- description: ''
  name: finding
  type: object
- description: ''
  name: findingReasonCodes
  type: object
- description: ''
  name: utilizationMetrics
  type: object
- description: ''
  name: lookBackPeriodInDays
  type: object
- description: ''
  name: recommendationOptions
  type: object
- description: ''
  name: recommendationSources
  type: object
- description: ''
  name: lastRefreshTimestamp
  type: object
- description: ''
  name: currentPerformanceRisk
  type: object
- description: ''
  name: effectiveRecommendationPreferences
  type: object
- description: ''
  name: inferredWorkloadTypes
  type: object
- description: ''
  name: instanceState
  type: object
- description: ''
  name: tags
  type: object
- description: ''
  name: externalMetricStatus
  type: object
provider_name: Amazon Compute Optimizer
provider_slug: amazon-compute-optimizer
schema_file: json-schema/compute-optimizer-instance-recommendation-schema.json
slug: compute-optimizer-instance-recommendation
source_filename: compute-optimizer-instance-recommendation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-instance-recommendation-schema.json\",\n  \"title\": \"InstanceRecommendation\",\n  \"description\": \"Describes an Amazon EC2 instance recommendation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the current instance.\"\n        }\n      ]\n    },\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID of the instance.\"\n        }\n      ]\n    },\n    \"instanceName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceName\"\
  \n        },\n        {\n          \"description\": \"The name of the current instance.\"\n        }\n      ]\n    },\n    \"currentInstanceType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CurrentInstanceType\"\n        },\n        {\n          \"description\": \"The instance type of the current instance.\"\n        }\n      ]\n    },\n    \"finding\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Finding\"\n        },\n        {\n          \"description\": \"<p>The finding classification of the instance.</p> <p>Findings for instances include:</p> <ul> <li> <p> <b> <code>Underprovisioned</code> </b>\\u2014An instance is considered under-provisioned when at least one specification of your instance, such as CPU, memory, or network, does not meet the performance requirements of your workload. Under-provisioned instances may lead to poor application performance.</p> </li> <li> <p> <b> <code>Overprovisioned</code> </b>\\u2014An\
  \ instance is considered over-provisioned when at least one specification of your instance, such as CPU, memory, or network, can be sized down while still meeting the performance requirements of your workload, and no specification is under-provisioned. Over-provisioned instances may lead to unnecessary infrastructure cost.</p> </li> <li> <p> <b> <code>Optimized</code> </b>\\u2014An instance is considered optimized when all specifications of your instance, such as CPU, memory, and network, meet the performance requirements of your workload and is not over provisioned. For optimized resources, Compute Optimizer might recommend a new generation instance type.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"findingReasonCodes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceRecommendationFindingReasonCodes\"\n        },\n        {\n          \"description\": \"<p>The reason for the finding classification of the instance.</p> <p>Finding reason codes\
  \ for instances include:</p> <ul> <li> <p> <b> <code>CPUOverprovisioned</code> </b> \\u2014 The instance\\u2019s CPU configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>CPUUtilization</code> metric of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>CPUUnderprovisioned</code> </b> \\u2014 The instance\\u2019s CPU configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better CPU performance. This is identified by analyzing the <code>CPUUtilization</code> metric of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>MemoryOverprovisioned</code> </b> \\u2014 The instance\\u2019s memory configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the memory utilization metric of the current instance during\
  \ the look-back period.</p> </li> <li> <p> <b> <code>MemoryUnderprovisioned</code> </b> \\u2014 The instance\\u2019s memory configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better memory performance. This is identified by analyzing the memory utilization metric of the current instance during the look-back period.</p> <note> <p>Memory utilization is analyzed only for resources that have the unified CloudWatch agent installed on them. For more information, see <a href=\\\"https://docs.aws.amazon.com/compute-optimizer/latest/ug/metrics.html#cw-agent\\\">Enabling memory utilization with the Amazon CloudWatch Agent</a> in the <i>Compute Optimizer User Guide</i>. On Linux instances, Compute Optimizer analyses the <code>mem_used_percent</code> metric in the <code>CWAgent</code> namespace, or the legacy <code>MemoryUtilization</code> metric in the <code>System/Linux</code> namespace. On Windows instances, Compute Optimizer\
  \ analyses the <code>Memory % Committed Bytes In Use</code> metric in the <code>CWAgent</code> namespace.</p> </note> </li> <li> <p> <b> <code>EBSThroughputOverprovisioned</code> </b> \\u2014 The instance\\u2019s EBS throughput configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>VolumeReadBytes</code> and <code>VolumeWriteBytes</code> metrics of EBS volumes attached to the current instance during the look-back period.</p> </li> <li> <p> <b> <code>EBSThroughputUnderprovisioned</code> </b> \\u2014 The instance\\u2019s EBS throughput configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better EBS throughput performance. This is identified by analyzing the <code>VolumeReadBytes</code> and <code>VolumeWriteBytes</code> metrics of EBS volumes attached to the current instance during the look-back period.</p> </li> <li> <p> <b> <code>EBSIOPSOverprovisioned</code>\
  \ </b> \\u2014 The instance\\u2019s EBS IOPS configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>VolumeReadOps</code> and <code>VolumeWriteOps</code> metric of EBS volumes attached to the current instance during the look-back period.</p> </li> <li> <p> <b> <code>EBSIOPSUnderprovisioned</code> </b> \\u2014 The instance\\u2019s EBS IOPS configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better EBS IOPS performance. This is identified by analyzing the <code>VolumeReadOps</code> and <code>VolumeWriteOps</code> metric of EBS volumes attached to the current instance during the look-back period.</p> </li> <li> <p> <b> <code>NetworkBandwidthOverprovisioned</code> </b> \\u2014 The instance\\u2019s network bandwidth configuration can be sized down while still meeting the performance requirements of your workload. This is identified\
  \ by analyzing the <code>NetworkIn</code> and <code>NetworkOut</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>NetworkBandwidthUnderprovisioned</code> </b> \\u2014 The instance\\u2019s network bandwidth configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better network bandwidth performance. This is identified by analyzing the <code>NetworkIn</code> and <code>NetworkOut</code> metrics of the current instance during the look-back period. This finding reason happens when the <code>NetworkIn</code> or <code>NetworkOut</code> performance of an instance is impacted.</p> </li> <li> <p> <b> <code>NetworkPPSOverprovisioned</code> </b> \\u2014 The instance\\u2019s network PPS (packets per second) configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>NetworkPacketsIn</code> and <code>NetworkPacketsIn</code>\
  \ metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>NetworkPPSUnderprovisioned</code> </b> \\u2014 The instance\\u2019s network PPS (packets per second) configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better network PPS performance. This is identified by analyzing the <code>NetworkPacketsIn</code> and <code>NetworkPacketsIn</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>DiskIOPSOverprovisioned</code> </b> \\u2014 The instance\\u2019s disk IOPS configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>DiskReadOps</code> and <code>DiskWriteOps</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>DiskIOPSUnderprovisioned</code> </b> \\u2014 The instance\\u2019s disk IOPS configuration doesn't meet\
  \ the performance requirements of your workload and there is an alternative instance type that provides better disk IOPS performance. This is identified by analyzing the <code>DiskReadOps</code> and <code>DiskWriteOps</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>DiskThroughputOverprovisioned</code> </b> \\u2014 The instance\\u2019s disk throughput configuration can be sized down while still meeting the performance requirements of your workload. This is identified by analyzing the <code>DiskReadBytes</code> and <code>DiskWriteBytes</code> metrics of the current instance during the look-back period.</p> </li> <li> <p> <b> <code>DiskThroughputUnderprovisioned</code> </b> \\u2014 The instance\\u2019s disk throughput configuration doesn't meet the performance requirements of your workload and there is an alternative instance type that provides better disk throughput performance. This is identified by analyzing the <code>DiskReadBytes</code>\
  \ and <code>DiskWriteBytes</code> metrics of the current instance during the look-back period.</p> </li> </ul> <note> <p>For more information about instance metrics, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/viewing_metrics_with_cloudwatch.html\\\">List the available CloudWatch metrics for your instances</a> in the <i>Amazon Elastic Compute Cloud User Guide</i>. For more information about EBS volume metrics, see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using_cloudwatch_ebs.html\\\">Amazon CloudWatch metrics for Amazon EBS</a> in the <i>Amazon Elastic Compute Cloud User Guide</i>.</p> </note>\"\n        }\n      ]\n    },\n    \"utilizationMetrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UtilizationMetrics\"\n        },\n        {\n          \"description\": \"An array of objects that describe the utilization metrics of the instance.\"\n        }\n      ]\n    },\n    \"lookBackPeriodInDays\": {\n  \
  \    \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LookBackPeriodInDays\"\n        },\n        {\n          \"description\": \"The number of days for which utilization metrics were analyzed for the instance.\"\n        }\n      ]\n    },\n    \"recommendationOptions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationOptions\"\n        },\n        {\n          \"description\": \"An array of objects that describe the recommendation options for the instance.\"\n        }\n      ]\n    },\n    \"recommendationSources\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecommendationSources\"\n        },\n        {\n          \"description\": \"An array of objects that describe the source resource of the recommendation.\"\n        }\n      ]\n    },\n    \"lastRefreshTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LastRefreshTimestamp\"\n        },\n       \
  \ {\n          \"description\": \"The timestamp of when the instance recommendation was last generated.\"\n        }\n      ]\n    },\n    \"currentPerformanceRisk\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CurrentPerformanceRisk\"\n        },\n        {\n          \"description\": \"The risk of the current instance not meeting the performance needs of its workloads. The higher the risk, the more likely the current instance cannot meet the performance requirements of its workload.\"\n        }\n      ]\n    },\n    \"effectiveRecommendationPreferences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EffectiveRecommendationPreferences\"\n        },\n        {\n          \"description\": \"An object that describes the effective recommendation preferences for the instance.\"\n        }\n      ]\n    },\n    \"inferredWorkloadTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InferredWorkloadTypes\"\
  \n        },\n        {\n          \"description\": \"<p>The applications that might be running on the instance as inferred by Compute Optimizer.</p> <p>Compute Optimizer can infer if one of the following applications might be running on the instance:</p> <ul> <li> <p> <code>AmazonEmr</code> - Infers that Amazon EMR might be running on the instance.</p> </li> <li> <p> <code>ApacheCassandra</code> - Infers that Apache Cassandra might be running on the instance.</p> </li> <li> <p> <code>ApacheHadoop</code> - Infers that Apache Hadoop might be running on the instance.</p> </li> <li> <p> <code>Memcached</code> - Infers that Memcached might be running on the instance.</p> </li> <li> <p> <code>NGINX</code> - Infers that NGINX might be running on the instance.</p> </li> <li> <p> <code>PostgreSql</code> - Infers that PostgreSQL might be running on the instance.</p> </li> <li> <p> <code>Redis</code> - Infers that Redis might be running on the instance.</p> </li> <li> <p> <code>Kafka</code> - Infers\
  \ that Kafka might be running on the instance.</p> </li> <li> <p> <code>SQLServer</code> - Infers that SQLServer might be running on the instance.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"instanceState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceState\"\n        },\n        {\n          \"description\": \" The state of the instance when the recommendation was generated. \"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \" A list of tags assigned to your Amazon EC2 instance recommendations. \"\n        }\n      ]\n    },\n    \"externalMetricStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalMetricStatus\"\n        },\n        {\n          \"description\": \" An object that describes Compute Optimizer's integration status with your external metrics provider. \"\
  \n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-compute-optimizer/refs/heads/main/json-schema/compute-optimizer-instance-recommendation-schema.json
tags:
- Cost Optimization
- FinOps
- Machine Learning
- Resource Recommendations
title: InstanceRecommendation
---
