---
description: <p>The number of worlds that will be created. You can configure the number of unique floorplans and the number of unique interiors for each floor plan. For example, if you want 1 world with 20 unique interiors, you set <code>floorplanCount = 1</code> and <code>interiorCountPerFloorplan = 20</code>. This will result in 20 worlds (<code>floorplanCount</code> * <code>interiorCountPerFloorplan)</code>. </p> <p>If you set <code>floorplanCount = 4</code> and <code>interiorCountPerFloorplan = 5</code>, there will be 20 worlds with 5 unique floor plans. </p>
layout: schema
name: WorldCount
properties_list:
- description: ''
  name: floorplanCount
  type: object
- description: ''
  name: interiorCountPerFloorplan
  type: object
provider_name: Amazon RoboMaker
provider_slug: amazon-robomaker
schema_file: json-schema/amazon-robomaker-openapi-world-count-schema.json
slug: amazon-robomaker-openapi-world-count
source_filename: amazon-robomaker-openapi-world-count-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-world-count-schema.json\",\n  \"title\": \"WorldCount\",\n  \"description\": \"<p>The number of worlds that will be created. You can configure the number of unique floorplans and the number of unique interiors for each floor plan. For example, if you want 1 world with 20 unique interiors, you set <code>floorplanCount = 1</code> and <code>interiorCountPerFloorplan = 20</code>. This will result in 20 worlds (<code>floorplanCount</code> * <code>interiorCountPerFloorplan)</code>. </p> <p>If you set <code>floorplanCount = 4</code> and <code>interiorCountPerFloorplan = 5</code>, there will be 20 worlds with 5 unique floor plans. </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"floorplanCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FloorplanCount\"\
  \n        },\n        {\n          \"description\": \"The number of unique floorplans.\"\n        }\n      ]\n    },\n    \"interiorCountPerFloorplan\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InteriorCountPerFloorplan\"\n        },\n        {\n          \"description\": \"The number of unique interiors per floorplan.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-robomaker/refs/heads/main/json-schema/amazon-robomaker-openapi-world-count-schema.json
tags:
- AWS
- Robotics
- Simulation
title: WorldCount
---
