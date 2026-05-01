---
description: Represents a Metadata Change Log event emitted when any aspect on the DataHub metadata graph is changed. This includes creates, updates, and removals of both versioned aspects (ownership, tags, glossary terms) and time-series aspects (dataset profiles, quality assertions). These events are consumed by the DataHub Actions Framework to trigger downstream processing pipelines.
layout: schema
name: DataHub Metadata Change Log Event
properties_list:
- description: The unique URN identifier for the entity being changed. Follows the format urn:li:{entityType}:{key}.
  name: entityUrn
  type: string
- description: The type of the entity being changed. Corresponds to one of the entity types registered in the DataHub metadata model.
  name: entityType
  type: string
- description: The type of change that occurred on the aspect. UPSERT indicates a create or update, DELETE indicates removal, CREATE indicates first-time creation, and RESTATE indicates a re-emission without modific
  name: changeType
  type: string
- description: The name of the entity aspect that was changed. Each aspect represents a specific facet of metadata such as properties, ownership, tags, or schema information.
  name: aspectName
  type: string
- description: The new aspect value after the change. Contains the JSON-serialized aspect payload and its content type.
  name: aspect
  type: object
- description: The previous aspect value before the change. Null if this is the first time the aspect is being set for the entity.
  name: previousAspectValue
  type: object
- description: System-level metadata associated with this change, including ingestion run identifiers and model registry information.
  name: systemMetadata
  type: object
- description: Audit stamp recording who made the change and when.
  name: created
  type: object
provider_name: DataHub
provider_slug: datahub
schema_file: json-schema/datahub-metadata-change-log-event-schema.json
slug: datahub-metadata-change-log-event
source_filename: datahub-metadata-change-log-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/datahub/json-schema/datahub-metadata-change-log-event-schema.json\",\n  \"title\": \"DataHub Metadata Change Log Event\",\n  \"description\": \"Represents a Metadata Change Log event emitted when any aspect on the DataHub metadata graph is changed. This includes creates, updates, and removals of both versioned aspects (ownership, tags, glossary terms) and time-series aspects (dataset profiles, quality assertions). These events are consumed by the DataHub Actions Framework to trigger downstream processing pipelines.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"entityUrn\",\n    \"entityType\",\n    \"changeType\",\n    \"aspectName\"\n  ],\n  \"properties\": {\n    \"entityUrn\": {\n      \"type\": \"string\",\n      \"description\": \"The unique URN identifier for the entity being changed. Follows the format urn:li:{entityType}:{key}.\",\n      \"pattern\"\
  : \"^urn:li:[a-zA-Z]+:.+$\",\n      \"examples\": [\n        \"urn:li:dataset:(urn:li:dataPlatform:hive,SampleHiveDataset,PROD)\",\n        \"urn:li:chart:(looker,dashboard_elements.1)\",\n        \"urn:li:dashboard:(looker,dashboards.1)\"\n      ]\n    },\n    \"entityType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the entity being changed. Corresponds to one of the entity types registered in the DataHub metadata model.\",\n      \"enum\": [\n        \"dataset\",\n        \"chart\",\n        \"dashboard\",\n        \"dataFlow\",\n        \"dataJob\",\n        \"corpUser\",\n        \"corpGroup\",\n        \"tag\",\n        \"domain\",\n        \"glossaryTerm\",\n        \"glossaryNode\",\n        \"container\",\n        \"dataPlatform\",\n        \"mlModel\",\n        \"mlModelGroup\",\n        \"mlFeature\",\n        \"mlFeatureTable\",\n        \"mlPrimaryKey\",\n        \"dataProduct\",\n        \"notebook\",\n        \"dataHubPolicy\",\n        \"dataHubRole\"\
  \n      ]\n    },\n    \"changeType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of change that occurred on the aspect. UPSERT indicates a create or update, DELETE indicates removal, CREATE indicates first-time creation, and RESTATE indicates a re-emission without modification.\",\n      \"enum\": [\n        \"UPSERT\",\n        \"DELETE\",\n        \"CREATE\",\n        \"RESTATE\"\n      ]\n    },\n    \"aspectName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the entity aspect that was changed. Each aspect represents a specific facet of metadata such as properties, ownership, tags, or schema information.\",\n      \"examples\": [\n        \"datasetProperties\",\n        \"schemaMetadata\",\n        \"ownership\",\n        \"globalTags\",\n        \"glossaryTerms\",\n        \"status\",\n        \"editableDatasetProperties\",\n        \"upstreamLineage\",\n        \"institutionalMemory\",\n        \"datasetKey\"\n      ]\n    },\n    \"\
  aspect\": {\n      \"$ref\": \"#/$defs/SerializedAspect\",\n      \"description\": \"The new aspect value after the change. Contains the JSON-serialized aspect payload and its content type.\"\n    },\n    \"previousAspectValue\": {\n      \"$ref\": \"#/$defs/SerializedAspect\",\n      \"description\": \"The previous aspect value before the change. Null if this is the first time the aspect is being set for the entity.\"\n    },\n    \"systemMetadata\": {\n      \"$ref\": \"#/$defs/SystemMetadata\",\n      \"description\": \"System-level metadata associated with this change, including ingestion run identifiers and model registry information.\"\n    },\n    \"created\": {\n      \"$ref\": \"#/$defs/AuditStamp\",\n      \"description\": \"Audit stamp recording who made the change and when.\"\n    }\n  },\n  \"$defs\": {\n    \"SerializedAspect\": {\n      \"type\": \"object\",\n      \"description\": \"A serialized aspect value containing the content type and the JSON-encoded aspect payload.\
  \ The value field contains a JSON string representing the aspect following its PDL schema definition.\",\n      \"required\": [\n        \"contentType\",\n        \"value\"\n      ],\n      \"properties\": {\n        \"contentType\": {\n          \"type\": \"string\",\n          \"description\": \"The MIME type of the serialized aspect value.\",\n          \"enum\": [\n            \"application/json\"\n          ]\n        },\n        \"value\": {\n          \"type\": \"string\",\n          \"description\": \"The JSON-serialized aspect value as a string. The structure of the JSON depends on the aspect name and follows the corresponding PDL schema definition.\"\n        }\n      }\n    },\n    \"SystemMetadata\": {\n      \"type\": \"object\",\n      \"description\": \"System-level metadata providing provenance and tracking information for a metadata change.\",\n      \"properties\": {\n        \"runId\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of\
  \ the ingestion run that produced this change. Used to correlate changes across a single ingestion execution.\"\n        },\n        \"lastObserved\": {\n          \"type\": \"integer\",\n          \"description\": \"The timestamp when this metadata was last observed, in epoch milliseconds.\",\n          \"minimum\": 0\n        },\n        \"registryName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the model registry associated with this change.\"\n        },\n        \"registryVersion\": {\n          \"type\": \"string\",\n          \"description\": \"The version of the model registry.\"\n        }\n      }\n    },\n    \"AuditStamp\": {\n      \"type\": \"object\",\n      \"description\": \"An audit stamp recording the actor and timestamp of a metadata modification.\",\n      \"required\": [\n        \"time\",\n        \"actor\"\n      ],\n      \"properties\": {\n        \"time\": {\n          \"type\": \"integer\",\n          \"description\": \"The\
  \ timestamp of the change in epoch milliseconds.\",\n          \"minimum\": 0\n        },\n        \"actor\": {\n          \"type\": \"string\",\n          \"description\": \"The URN of the actor who made the change.\",\n          \"pattern\": \"^urn:li:corpuser:.+$\",\n          \"examples\": [\n            \"urn:li:corpuser:datahub\",\n            \"urn:li:corpuser:admin\"\n          ]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datahub/refs/heads/main/json-schema/datahub-metadata-change-log-event-schema.json
tags:
- Data Catalog
- Data Discovery
- Data Governance
- Data Lineage
- Metadata
title: DataHub Metadata Change Log Event
---
