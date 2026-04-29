---
description: Records configuration changes to specified resource types. For more information about the configuration recorder, see <a href="https://docs.aws.amazon.com/config/latest/developerguide/stop-start-recorder.html"> <b>Managing the Configuration Recorder</b> </a> in the <i>Config Developer Guide</i>.
layout: schema
name: ConfigurationRecorder
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: roleARN
  type: object
- description: ''
  name: recordingGroup
  type: object
provider_name: Amazon Config
provider_slug: amazon-config
schema_file: json-schema/config-configuration-recorder-schema.json
slug: config-configuration-recorder
source_filename: config-configuration-recorder-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-configuration-recorder-schema.json\",\n  \"title\": \"ConfigurationRecorder\",\n  \"description\": \"Records configuration changes to specified resource types. For more information about the configuration recorder, see <a href=\\\"https://docs.aws.amazon.com/config/latest/developerguide/stop-start-recorder.html\\\"> <b>Managing the Configuration Recorder</b> </a> in the <i>Config Developer Guide</i>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecorderName\"\n        },\n        {\n          \"description\": \"<p>The name of the configuration recorder. Config automatically assigns the name of \\\"default\\\" when creating the configuration recorder.</p> <p>You cannot change the name of the configuration\
  \ recorder after it has been created. To change the configuration recorder name, you must delete it and create a new configuration recorder with a new name. </p>\"\n        }\n      ]\n    },\n    \"roleARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"<p>Amazon Resource Name (ARN) of the IAM role assumed by Config and used by the configuration recorder.</p> <note> <p>While the API model does not require this field, the server will reject a request without a defined <code>roleARN</code> for the configuration recorder.</p> </note> <note> <p> <b>Pre-existing Config role</b> </p> <p>If you have used an Amazon Web Services service that uses Config, such as Security Hub or Control Tower, and an Config role has already been created, make sure that the IAM role that you use when setting up Config keeps the same minimum permissions as the already created Config role. You must do this so that the other\
  \ Amazon Web Services service continues to run as expected. </p> <p>For example, if Control Tower has an IAM role that allows Config to read Amazon Simple Storage Service (Amazon S3) objects, make sure that the same permissions are granted within the IAM role you use when setting up Config. Otherwise, it may interfere with how Control Tower operates. For more information about IAM roles for Config, see <a href=\\\"https://docs.aws.amazon.com/config/latest/developerguide/security-iam.html\\\"> <b>Identity and Access Management for Config</b> </a> in the <i>Config Developer Guide</i>. </p> </note>\"\n        }\n      ]\n    },\n    \"recordingGroup\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordingGroup\"\n        },\n        {\n          \"description\": \"<p>Specifies which resource types Config records for configuration changes.</p> <note> <p> <b> High Number of Config Evaluations</b> </p> <p>You may notice increased activity in your account during\
  \ your initial month recording with Config when compared to subsequent months. During the initial bootstrapping process, Config runs evaluations on all the resources in your account that you have selected for Config to record.</p> <p>If you are running ephemeral workloads, you may see increased activity from Config as it records configuration changes associated with creating and deleting these temporary resources. An <i>ephemeral workload</i> is a temporary use of computing resources that are loaded and run when needed. Examples include Amazon Elastic Compute Cloud (Amazon EC2) Spot Instances, Amazon EMR jobs, and Auto Scaling. If you want to avoid the increased activity from running ephemeral workloads, you can run these types of workloads in a separate account with Config turned off to avoid increased configuration recording and rule evaluations.</p> </note>\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-config/refs/heads/main/json-schema/config-configuration-recorder-schema.json
tags:
- Auditing
- AWS
- Compliance
- Configuration Management
- Governance
- Security
title: ConfigurationRecorder
---
