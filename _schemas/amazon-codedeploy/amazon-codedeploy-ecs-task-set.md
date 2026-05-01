---
description: Information about a set of Amazon ECS tasks in an CodeDeploy deployment. An Amazon ECS task set includes details such as the desired number of tasks, how many tasks are running, and whether the task set serves production traffic. An CodeDeploy application that uses the Amazon ECS compute platform deploys a containerized application in an Amazon ECS service as a task set.
layout: schema
name: ECSTaskSet
properties_list:
- description: ''
  name: identifer
  type: object
- description: ''
  name: desiredCount
  type: object
- description: ''
  name: pendingCount
  type: object
- description: ''
  name: runningCount
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: trafficWeight
  type: object
- description: ''
  name: targetGroup
  type: object
- description: ''
  name: taskSetLabel
  type: object
provider_name: Amazon CodeDeploy
provider_slug: amazon-codedeploy
schema_file: json-schema/amazon-codedeploy-ecs-task-set-schema.json
slug: amazon-codedeploy-ecs-task-set
source_filename: amazon-codedeploy-ecs-task-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-ecs-task-set-schema.json\",\n  \"title\": \"ECSTaskSet\",\n  \"description\": \" Information about a set of Amazon ECS tasks in an CodeDeploy deployment. An Amazon ECS task set includes details such as the desired number of tasks, how many tasks are running, and whether the task set serves production traffic. An CodeDeploy application that uses the Amazon ECS compute platform deploys a containerized application in an Amazon ECS service as a task set. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"identifer\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSTaskSetIdentifier\"\n        },\n        {\n          \"description\": \" A unique ID of an <code>ECSTaskSet</code>. \"\n        }\n      ]\n    },\n    \"desiredCount\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/ECSTaskSetCount\"\n        },\n        {\n          \"description\": \" The number of tasks in a task set. During a deployment that uses the Amazon ECS compute type, CodeDeploy instructs Amazon ECS to create a new task set and uses this value to determine how many tasks to create. After the updated task set is created, CodeDeploy shifts traffic to the new task set. \"\n        }\n      ]\n    },\n    \"pendingCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSTaskSetCount\"\n        },\n        {\n          \"description\": \" The number of tasks in the task set that are in the <code>PENDING</code> status during an Amazon ECS deployment. A task in the <code>PENDING</code> state is preparing to enter the <code>RUNNING</code> state. A task set enters the <code>PENDING</code> status when it launches for the first time, or when it is restarted after being in the <code>STOPPED</code> state. \"\n\
  \        }\n      ]\n    },\n    \"runningCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSTaskSetCount\"\n        },\n        {\n          \"description\": \" The number of tasks in the task set that are in the <code>RUNNING</code> status during an Amazon ECS deployment. A task in the <code>RUNNING</code> state is running and ready for use. \"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ECSTaskSetStatus\"\n        },\n        {\n          \"description\": \"<p> The status of the task set. There are three valid task set statuses: </p> <ul> <li> <p> <code>PRIMARY</code>: Indicates the task set is serving production traffic. </p> </li> <li> <p> <code>ACTIVE</code>: Indicates the task set is not serving production traffic. </p> </li> <li> <p> <code>DRAINING</code>: Indicates the tasks in the task set are being stopped and their corresponding targets are being deregistered\
  \ from their target group. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"trafficWeight\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TrafficWeight\"\n        },\n        {\n          \"description\": \" The percentage of traffic served by this task set. \"\n        }\n      ]\n    },\n    \"targetGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetGroupInfo\"\n        },\n        {\n          \"description\": \" The target group associated with the task set. The target group is used by CodeDeploy to manage traffic to a task set. \"\n        }\n      ]\n    },\n    \"taskSetLabel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetLabel\"\n        },\n        {\n          \"description\": \" A label that identifies whether the ECS task set is an original target (<code>BLUE</code>) or a replacement target (<code>GREEN</code>). \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codedeploy/refs/heads/main/json-schema/amazon-codedeploy-ecs-task-set-schema.json
tags:
- Amazon
- Deployment
- DevOps
- CI/CD
- Release Management
- Blue/Green Deployment
title: ECSTaskSet
---
