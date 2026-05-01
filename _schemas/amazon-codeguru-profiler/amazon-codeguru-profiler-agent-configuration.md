---
description: The response of <a href="https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_ConfigureAgent.html"> <code>ConfigureAgent</code> </a> that specifies if an agent profiles or not and for how long to return profiling data.
layout: schema
name: AgentConfiguration
properties_list:
- description: ''
  name: agentParameters
  type: object
- description: ''
  name: periodInSeconds
  type: object
- description: ''
  name: shouldProfile
  type: object
provider_name: Amazon CodeGuru Profiler
provider_slug: amazon-codeguru-profiler
schema_file: json-schema/amazon-codeguru-profiler-agent-configuration-schema.json
slug: amazon-codeguru-profiler-agent-configuration
source_filename: amazon-codeguru-profiler-agent-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-agent-configuration-schema.json\",\n  \"title\": \"AgentConfiguration\",\n  \"description\": \" The response of <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_ConfigureAgent.html\\\"> <code>ConfigureAgent</code> </a> that specifies if an agent profiles or not and for how long to return profiling data. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agentParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AgentParameters\"\n        },\n        {\n          \"description\": \"<p> Parameters used by the profiler. The valid parameters are: </p> <ul> <li> <p> <code>MaxStackDepth</code> - The maximum depth of the stacks in the code that is represented in the profile. For example, if CodeGuru Profiler finds\
  \ a method <code>A</code>, which calls method <code>B</code>, which calls method <code>C</code>, which calls method <code>D</code>, then the depth is 4. If the <code>maxDepth</code> is set to 2, then the profiler evaluates <code>A</code> and <code>B</code>. </p> </li> <li> <p> <code>MemoryUsageLimitPercent</code> - The percentage of memory that is used by the profiler.</p> </li> <li> <p> <code>MinimumTimeForReportingInMilliseconds</code> - The minimum time in milliseconds between sending reports. </p> </li> <li> <p> <code>ReportingIntervalInMilliseconds</code> - The reporting interval in milliseconds used to report profiles. </p> </li> <li> <p> <code>SamplingIntervalInMilliseconds</code> - The sampling interval in milliseconds that is used to profile samples. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"periodInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \" How long a profiling\
  \ agent should send profiling data using <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_ConfigureAgent.html\\\"> <code>ConfigureAgent</code> </a>. For example, if this is set to 300, the profiling agent calls <a href=\\\"https://docs.aws.amazon.com/codeguru/latest/profiler-api/API_ConfigureAgent.html\\\"> <code>ConfigureAgent</code> </a> every 5 minutes to submit the profiled data collected during that period. \"\n        }\n      ]\n    },\n    \"shouldProfile\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \" A <code>Boolean</code> that specifies whether the profiling agent collects profiling data or not. Set to <code>true</code> to enable profiling. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"periodInSeconds\",\n    \"shouldProfile\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codeguru-profiler/refs/heads/main/json-schema/amazon-codeguru-profiler-agent-configuration-schema.json
tags:
- Amazon
- Application Performance
- Profiling
- DevOps
- Machine Learning
title: AgentConfiguration
---
