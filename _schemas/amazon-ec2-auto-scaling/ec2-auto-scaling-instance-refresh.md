---
description: Describes an instance refresh for an Auto Scaling group.
layout: schema
name: InstanceRefresh
properties_list:
- description: ''
  name: InstanceRefreshId
  type: object
- description: ''
  name: AutoScalingGroupName
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: StatusReason
  type: object
- description: ''
  name: StartTime
  type: object
- description: ''
  name: EndTime
  type: object
- description: ''
  name: PercentageComplete
  type: object
- description: ''
  name: InstancesToUpdate
  type: object
- description: ''
  name: ProgressDetails
  type: object
- description: ''
  name: Preferences
  type: object
- description: ''
  name: DesiredConfiguration
  type: object
- description: ''
  name: RollbackDetails
  type: object
provider_name: Amazon EC2 Auto Scaling
provider_slug: amazon-ec2-auto-scaling
schema_file: json-schema/ec2-auto-scaling-instance-refresh-schema.json
slug: ec2-auto-scaling-instance-refresh
source_filename: ec2-auto-scaling-instance-refresh-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-instance-refresh-schema.json\",\n  \"title\": \"InstanceRefresh\",\n  \"description\": \"Describes an instance refresh for an Auto Scaling group. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceRefreshId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The instance refresh ID.\"\n        }\n      ]\n    },\n    \"AutoScalingGroupName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen255\"\n        },\n        {\n          \"description\": \"The name of the Auto Scaling group.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceRefreshStatus\"\
  \n        },\n        {\n          \"description\": \"<p>The current status for the instance refresh operation:</p> <ul> <li> <p> <code>Pending</code> - The request was created, but the instance refresh has not started.</p> </li> <li> <p> <code>InProgress</code> - An instance refresh is in progress.</p> </li> <li> <p> <code>Successful</code> - An instance refresh completed successfully.</p> </li> <li> <p> <code>Failed</code> - An instance refresh failed to complete. You can troubleshoot using the status reason and the scaling activities. </p> </li> <li> <p> <code>Cancelling</code> - An ongoing instance refresh is being cancelled.</p> </li> <li> <p> <code>Cancelled</code> - The instance refresh is cancelled. </p> </li> <li> <p> <code>RollbackInProgress</code> - An instance refresh is being rolled back.</p> </li> <li> <p> <code>RollbackFailed</code> - The rollback failed to complete. You can troubleshoot using the status reason and the scaling activities.</p> </li> <li> <p> <code>RollbackSuccessful</code>\
  \ - The rollback completed successfully.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"StatusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/XmlStringMaxLen1023\"\n        },\n        {\n          \"description\": \"The explanation for the specific status assigned to this operation.\"\n        }\n      ]\n    },\n    \"StartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampType\"\n        },\n        {\n          \"description\": \"The date and time at which the instance refresh began.\"\n        }\n      ]\n    },\n    \"EndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimestampType\"\n        },\n        {\n          \"description\": \"The date and time at which the instance refresh ended.\"\n        }\n      ]\n    },\n    \"PercentageComplete\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IntPercent\"\n        },\n       \
  \ {\n          \"description\": \"<p>The percentage of the instance refresh that is complete. For each instance replacement, Amazon EC2 Auto Scaling tracks the instance's health status and warm-up time. When the instance's health status changes to healthy and the specified warm-up time passes, the instance is considered updated and is added to the percentage complete.</p> <note> <p> <code>PercentageComplete</code> does not include instances that are replaced during a rollback. This value gradually goes back down to zero during a rollback.</p> </note>\"\n        }\n      ]\n    },\n    \"InstancesToUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstancesToUpdate\"\n        },\n        {\n          \"description\": \"<p>The number of instances remaining to update before the instance refresh is complete.</p> <note> <p>If you roll back the instance refresh, <code>InstancesToUpdate</code> shows you the number of instances that were not yet updated by\
  \ the instance refresh. Therefore, these instances don't need to be replaced as part of the rollback.</p> </note>\"\n        }\n      ]\n    },\n    \"ProgressDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceRefreshProgressDetails\"\n        },\n        {\n          \"description\": \"Additional progress details for an Auto Scaling group that has a warm pool.\"\n        }\n      ]\n    },\n    \"Preferences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RefreshPreferences\"\n        },\n        {\n          \"description\": \"The preferences for an instance refresh.\"\n        }\n      ]\n    },\n    \"DesiredConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DesiredConfiguration\"\n        },\n        {\n          \"description\": \"Describes the desired configuration for the instance refresh.\"\n        }\n      ]\n    },\n    \"RollbackDetails\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/RollbackDetails\"\n        },\n        {\n          \"description\": \"The rollback details.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-auto-scaling/refs/heads/main/json-schema/ec2-auto-scaling-instance-refresh-schema.json
tags:
- Amazon Web Services
- Auto Scaling
- Compute
- EC2
- High Availability
- Scaling
title: InstanceRefresh
---
