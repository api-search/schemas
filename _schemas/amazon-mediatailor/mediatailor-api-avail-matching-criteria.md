---
description: <p>MediaTailor only places (consumes) prefetched ads if the ad break meets the criteria defined by the dynamic variables. This gives you granular control over which ad break to place the prefetched ads into.</p> <p>As an example, let's say that you set <code>DynamicVariable</code> to <code>scte.event_id</code> and <code>Operator</code> to <code>EQUALS</code>, and your playback configuration has an ADS URL of <code>https://my.ads.server.com/path?&amp;podId=[scte.avail_num]&amp;event=[scte.event_id]&amp;duration=[session.avail_duration_secs]</code>. And the prefetch request to the ADS contains these values <code>https://my.ads.server.com/path?&amp;podId=3&amp;event=my-awesome-event&amp;duration=30</code>. MediaTailor will only insert the prefetched ads into the ad break if has a SCTE marker with an event id of <code>my-awesome-event</code>, since it must match the event id that MediaTailor uses to query the ADS.</p> <p>You can specify up to five <code>AvailMatchingCriteria</code>.
  If you specify multiple <code>AvailMatchingCriteria</code>, MediaTailor combines them to match using a logical <code>AND</code>. You can model logical <code>OR</code> combinations by creating multiple prefetch schedules.</p>
layout: schema
name: AvailMatchingCriteria
properties_list:
- description: ''
  name: DynamicVariable
  type: object
- description: ''
  name: Operator
  type: object
provider_name: Amazon MediaTailor
provider_slug: amazon-mediatailor
schema_file: json-schema/mediatailor-api-avail-matching-criteria-schema.json
slug: mediatailor-api-avail-matching-criteria
source_filename: mediatailor-api-avail-matching-criteria-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-avail-matching-criteria-schema.json\",\n  \"title\": \"AvailMatchingCriteria\",\n  \"description\": \"<p>MediaTailor only places (consumes) prefetched ads if the ad break meets the criteria defined by the dynamic variables. This gives you granular control over which ad break to place the prefetched ads into.</p> <p>As an example, let's say that you set <code>DynamicVariable</code> to <code>scte.event_id</code> and <code>Operator</code> to <code>EQUALS</code>, and your playback configuration has an ADS URL of <code>https://my.ads.server.com/path?&amp;podId=[scte.avail_num]&amp;event=[scte.event_id]&amp;duration=[session.avail_duration_secs]</code>. And the prefetch request to the ADS contains these values <code>https://my.ads.server.com/path?&amp;podId=3&amp;event=my-awesome-event&amp;duration=30</code>.\
  \ MediaTailor will only insert the prefetched ads into the ad break if has a SCTE marker with an event id of <code>my-awesome-event</code>, since it must match the event id that MediaTailor uses to query the ADS.</p> <p>You can specify up to five <code>AvailMatchingCriteria</code>. If you specify multiple <code>AvailMatchingCriteria</code>, MediaTailor combines them to match using a logical <code>AND</code>. You can model logical <code>OR</code> combinations by creating multiple prefetch schedules.</p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DynamicVariable\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/__string\"\n        },\n        {\n          \"description\": \"<p>The dynamic variable(s) that MediaTailor should use as avail matching criteria. MediaTailor only places the prefetched ads into the avail if the avail matches the criteria defined by the dynamic variable. For information about dynamic variables, see <a href=\\\"https://docs.aws.amazon.com/mediatailor/latest/ug/variables.html\\\
  \">Using dynamic ad variables</a> in the <i>MediaTailor User Guide</i>.</p> <p>You can include up to 100 dynamic variables.</p>\"\n        }\n      ]\n    },\n    \"Operator\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Operator\"\n        },\n        {\n          \"description\": \"For the <code>DynamicVariable</code> specified in <code>AvailMatchingCriteria</code>, the Operator that is used for the comparison.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"DynamicVariable\",\n    \"Operator\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-mediatailor/refs/heads/main/json-schema/mediatailor-api-avail-matching-criteria-schema.json
tags:
- Broadcasting
- Media Processing
- Media
title: AvailMatchingCriteria
---
