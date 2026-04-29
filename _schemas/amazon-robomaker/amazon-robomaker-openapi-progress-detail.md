---
description: Information about the progress of a deployment job.
layout: schema
name: ProgressDetail
properties_list:
- description: ''
  name: currentProgress
  type: object
- description: ''
  name: percentDone
  type: object
- description: ''
  name: estimatedTimeRemainingSeconds
  type: object
- description: ''
  name: targetResource
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-progress-detail-schema.json
slug: amazon-robomaker-openapi-progress-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-progress-detail-schema.json\",\n  \"title\": \"ProgressDetail\",\n  \"description\": \"Information about the progress of a deployment job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currentProgress\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RobotDeploymentStep\"\n        },\n        {\n          \"description\": \"<p>The current progress status.</p> <dl> <dt>Validating</dt> <dd> <p>Validating the deployment.</p> </dd> <dt>DownloadingExtracting</dt> <dd> <p>Downloading and extracting the bundle on the robot.</p> </dd> <dt>ExecutingPreLaunch</dt> <dd> <p>Executing pre-launch script(s) if provided.</p> </dd> <dt>Launching</dt> <dd> <p>Launching the robot application.</p> </dd> <dt>ExecutingPostLaunch</dt> <dd> <p>Executing post-launch\
  \ script(s) if provided.</p> </dd> <dt>Finished</dt> <dd> <p>Deployment is complete.</p> </dd> </dl>\"\n        }\n      ]\n    },\n    \"percentDone\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PercentDone\"\n        },\n        {\n          \"description\": \"Precentage of the step that is done. This currently only applies to the <code>Downloading/Extracting</code> step of the deployment. It is empty for other steps.\"\n        }\n      ]\n    },\n    \"estimatedTimeRemainingSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericInteger\"\n        },\n        {\n          \"description\": \"Estimated amount of time in seconds remaining in the step. This currently only applies to the <code>Downloading/Extracting</code> step of the deployment. It is empty for other steps.\"\n        }\n      ]\n    },\n    \"targetResource\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GenericString\"\
  \n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the deployment job.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-progress-detail-schema.json
tags:
- AWS
- Robotics
- Simulation
title: ProgressDetail
---
