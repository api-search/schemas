---
description: A schedule configures how often and when a pipeline will automatically create a new image.
layout: schema
name: Schedule
properties_list:
- description: ''
  name: scheduleExpression
  type: object
- description: ''
  name: timezone
  type: object
- description: ''
  name: pipelineExecutionStartCondition
  type: object
provider_name: Amazon EC2 Image Builder
provider_slug: amazon-ec2-image-builder
schema_file: json-schema/ec2-image-builder-schedule-schema.json
slug: ec2-image-builder-schedule
source_filename: ec2-image-builder-schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-schedule-schema.json\",\n  \"title\": \"Schedule\",\n  \"description\": \"A schedule configures how often and when a pipeline will automatically create a new image.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"scheduleExpression\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"<p>The cron expression determines how often EC2 Image Builder evaluates your <code>pipelineExecutionStartCondition</code>.</p> <p>For information on how to format a cron expression in Image Builder, see <a href=\\\"https://docs.aws.amazon.com/imagebuilder/latest/userguide/image-builder-cron.html\\\">Use cron expressions in EC2 Image Builder</a>.</p>\"\n        }\n      ]\n    },\n    \"timezone\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timezone\"\n        },\n        {\n          \"description\": \"The timezone that applies to the scheduling expression. For example, \\\"Etc/UTC\\\", \\\"America/Los_Angeles\\\" in the <a href=\\\"https://www.joda.org/joda-time/timezones.html\\\">IANA timezone format</a>. If not specified this defaults to UTC.\"\n        }\n      ]\n    },\n    \"pipelineExecutionStartCondition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineExecutionStartCondition\"\n        },\n        {\n          \"description\": \"The condition configures when the pipeline should trigger a new image build. When the <code>pipelineExecutionStartCondition</code> is set to <code>EXPRESSION_MATCH_AND_DEPENDENCY_UPDATES_AVAILABLE</code>, and you use semantic version filters on the base image or components in your image recipe, EC2 Image Builder will build a new image only when there are new versions of\
  \ the image or components in your recipe that match the semantic version filter. When it is set to <code>EXPRESSION_MATCH_ONLY</code>, it will build a new image every time the CRON expression matches the current time. For semantic version syntax, see <a href=\\\"https://docs.aws.amazon.com/imagebuilder/latest/APIReference/API_CreateComponent.html\\\">CreateComponent</a> in the <i> EC2 Image Builder API Reference</i>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ec2-image-builder/refs/heads/main/json-schema/ec2-image-builder-schedule-schema.json
tags:
- Amazon Web Services
- Automation
- Container Images
- EC2
- Image Building
- Virtual Machine Images
title: Schedule
---
