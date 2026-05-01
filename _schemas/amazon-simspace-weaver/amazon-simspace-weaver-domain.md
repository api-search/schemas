---
description: '<p>A collection of app instances that run the same executable app code and have the same launch options and commands.</p> <p>For more information about domains, see <a href="https://docs.aws.amazon.com/simspaceweaver/latest/userguide/what-is_key-concepts.html#what-is_key-concepts_domains">Key concepts: Domains</a> in the <i>SimSpace Weaver User Guide</i>.</p>'
layout: schema
name: Domain
properties_list:
- description: ''
  name: Lifecycle
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
schema_file: json-schema/amazon-simspace-weaver-domain-schema.json
slug: amazon-simspace-weaver-domain
source_filename: amazon-simspace-weaver-domain-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-domain-schema.json\",\n  \"title\": \"Domain\",\n  \"description\": \"<p>A collection of app instances that run the same executable app code and have the same launch options and commands.</p> <p>For more information about domains, see <a href=\\\"https://docs.aws.amazon.com/simspaceweaver/latest/userguide/what-is_key-concepts.html#what-is_key-concepts_domains\\\">Key concepts: Domains</a> in the <i>SimSpace Weaver User Guide</i>.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Lifecycle\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LifecycleManagementStrategy\"\n        },\n        {\n          \"description\": \"<p>The type of lifecycle management for apps in the domain. Indicates whether apps in this domain are <i>managed</i>\
  \ (SimSpace Weaver starts and stops the apps) or <i>unmanaged</i> (you must start and stop the apps).</p> <p class=\\\"title\\\"> <b>Lifecycle types</b> </p> <ul> <li> <p> <code>PerWorker</code> \\u2013 Managed: SimSpace Weaver starts one app on each worker.</p> </li> <li> <p> <code>BySpatialSubdivision</code> \\u2013 Managed: SimSpace Weaver starts one app for each spatial partition.</p> </li> <li> <p> <code>ByRequest</code> \\u2013 Unmanaged: You use the <code>StartApp</code> API to start the apps and use the <code>StopApp</code> API to stop the apps.</p> </li> </ul>\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SimSpaceWeaverResourceName\"\n        },\n        {\n          \"description\": \"The name of the domain.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/json-schema/amazon-simspace-weaver-domain-schema.json
tags:
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
title: Domain
---
