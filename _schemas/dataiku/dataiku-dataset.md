---
description: A dataset in Dataiku DSS representing a structured data source or output, including its schema, connection parameters, format configuration, and flow integration settings.
layout: schema
name: Dataiku DSS Dataset
properties_list:
- description: Project key that this dataset belongs to
  name: projectKey
  type: string
- description: Dataset name, unique within the project
  name: name
  type: string
- description: Type of the dataset, determining the underlying storage or connection
  name: type
  type: string
- description: Whether the dataset is managed by DSS (output of a recipe) or external
  name: managed
  type: boolean
- description: ''
  name: schema
  type: object
- description: Data format for file-based datasets
  name: formatType
  type: string
- description: Format-specific parameters
  name: formatParams
  type: object
- description: Type-specific connection and access parameters
  name: params
  type: object
- description: ''
  name: partitioning
  type: object
- description: Options for how this dataset behaves in the flow
  name: flowOptions
  type: object
- description: ''
  name: metrics
  type: object
- description: ''
  name: checks
  type: object
- description: ''
  name: creationTag
  type: object
- description: ''
  name: versionTag
  type: object
provider_name: Dataiku
provider_slug: dataiku
schema_file: json-schema/dataiku-dataset-schema.json
slug: dataiku-dataset
source_filename: dataiku-dataset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://doc.dataiku.com/schemas/dataiku/dataset.json\",\n  \"title\": \"Dataiku DSS Dataset\",\n  \"description\": \"A dataset in Dataiku DSS representing a structured data source or output, including its schema, connection parameters, format configuration, and flow integration settings.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"type\"],\n  \"properties\": {\n    \"projectKey\": {\n      \"type\": \"string\",\n      \"description\": \"Project key that this dataset belongs to\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Dataset name, unique within the project\",\n      \"minLength\": 1,\n      \"maxLength\": 256\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Filesystem\",\n        \"UploadedFiles\",\n        \"PostgreSQL\",\n        \"MySQL\",\n        \"Oracle\",\n        \"SQLServer\",\n        \"Redshift\"\
  ,\n        \"BigQuery\",\n        \"Snowflake\",\n        \"Synapse\",\n        \"Teradata\",\n        \"S3\",\n        \"GCS\",\n        \"Azure\",\n        \"HDFS\",\n        \"Hive\",\n        \"MongoDB\",\n        \"Elasticsearch\",\n        \"Cassandra\",\n        \"HTTP\",\n        \"FTP\",\n        \"SCP\",\n        \"Twitter\",\n        \"Inline\",\n        \"StatsDB\",\n        \"JobsDB\",\n        \"JDBC\"\n      ],\n      \"description\": \"Type of the dataset, determining the underlying storage or connection\"\n    },\n    \"managed\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the dataset is managed by DSS (output of a recipe) or external\"\n    },\n    \"schema\": {\n      \"$ref\": \"#/$defs/Schema\"\n    },\n    \"formatType\": {\n      \"type\": \"string\",\n      \"enum\": [\"csv\", \"parquet\", \"json\", \"avro\", \"orc\", \"excel\", \"xml\"],\n      \"description\": \"Data format for file-based datasets\"\n    },\n    \"formatParams\": {\n   \
  \   \"type\": \"object\",\n      \"description\": \"Format-specific parameters\",\n      \"properties\": {\n        \"separator\": {\n          \"type\": \"string\",\n          \"description\": \"Column separator for CSV files\"\n        },\n        \"style\": {\n          \"type\": \"string\",\n          \"description\": \"CSV style (e.g., excel, unix, escaped)\"\n        },\n        \"quoteChar\": {\n          \"type\": \"string\",\n          \"description\": \"Quote character for CSV\"\n        },\n        \"escapeChar\": {\n          \"type\": \"string\",\n          \"description\": \"Escape character for CSV\"\n        },\n        \"parseHeaderRow\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to parse the first row as header\"\n        },\n        \"charset\": {\n          \"type\": \"string\",\n          \"description\": \"Character encoding (e.g., utf8, latin1)\"\n        },\n        \"compress\": {\n          \"type\": \"string\",\n          \"description\"\
  : \"Compression type (e.g., gz, bz2, snappy)\"\n        }\n      }\n    },\n    \"params\": {\n      \"type\": \"object\",\n      \"description\": \"Type-specific connection and access parameters\",\n      \"properties\": {\n        \"connection\": {\n          \"type\": \"string\",\n          \"description\": \"DSS connection name for database-backed datasets\"\n        },\n        \"table\": {\n          \"type\": \"string\",\n          \"description\": \"Database table name\"\n        },\n        \"schema\": {\n          \"type\": \"string\",\n          \"description\": \"Database schema name\"\n        },\n        \"catalog\": {\n          \"type\": \"string\",\n          \"description\": \"Database catalog name\"\n        },\n        \"path\": {\n          \"type\": \"string\",\n          \"description\": \"File path for file-based datasets\"\n        },\n        \"bucket\": {\n          \"type\": \"string\",\n          \"description\": \"Cloud storage bucket name\"\n        },\n\
  \        \"notReadyIfEmpty\": {\n          \"type\": \"boolean\",\n          \"description\": \"Consider dataset not ready if it contains no data\"\n        }\n      }\n    },\n    \"partitioning\": {\n      \"$ref\": \"#/$defs/Partitioning\"\n    },\n    \"flowOptions\": {\n      \"type\": \"object\",\n      \"description\": \"Options for how this dataset behaves in the flow\",\n      \"properties\": {\n        \"virtualizable\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the dataset can be virtualized\"\n        },\n        \"rebuildBehavior\": {\n          \"type\": \"string\",\n          \"enum\": [\"NORMAL\", \"WRITE_PROTECTED\", \"NO_REBUILD\"],\n          \"description\": \"Rebuild behavior for the dataset\"\n        },\n        \"crossProjectBuildBehavior\": {\n          \"type\": \"string\",\n          \"enum\": [\"DEFAULT\", \"BUILD\", \"NO_BUILD\"],\n          \"description\": \"Build behavior when accessed from another project\"\n        }\n \
  \     }\n    },\n    \"metrics\": {\n      \"$ref\": \"#/$defs/MetricsSettings\"\n    },\n    \"checks\": {\n      \"$ref\": \"#/$defs/ChecksSettings\"\n    },\n    \"creationTag\": {\n      \"$ref\": \"#/$defs/VersionTag\"\n    },\n    \"versionTag\": {\n      \"$ref\": \"#/$defs/VersionTag\"\n    }\n  },\n  \"$defs\": {\n    \"Schema\": {\n      \"type\": \"object\",\n      \"description\": \"Dataset schema defining columns and their types\",\n      \"properties\": {\n        \"columns\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/Column\"\n          },\n          \"description\": \"Ordered list of columns\"\n        },\n        \"userModified\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the schema was manually modified by a user\"\n        }\n      }\n    },\n    \"Column\": {\n      \"type\": \"object\",\n      \"description\": \"A column in a dataset schema\",\n      \"required\": [\"name\", \"type\"],\n\
  \      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Column name\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"string\",\n            \"bigint\",\n            \"int\",\n            \"smallint\",\n            \"tinyint\",\n            \"double\",\n            \"float\",\n            \"boolean\",\n            \"date\",\n            \"array\",\n            \"map\",\n            \"object\",\n            \"geopoint\",\n            \"geometry\"\n          ],\n          \"description\": \"Column data type\"\n        },\n        \"meaning\": {\n          \"type\": \"string\",\n          \"description\": \"Semantic meaning assigned to this column (e.g., Email, URL, IPAddress)\"\n        },\n        \"maxLength\": {\n          \"type\": \"integer\",\n          \"minimum\": -1,\n          \"description\": \"Maximum length for string columns (-1 for unlimited)\"\n        },\n       \
  \ \"comment\": {\n          \"type\": \"string\",\n          \"description\": \"Documentation comment for the column\"\n        }\n      }\n    },\n    \"Partitioning\": {\n      \"type\": \"object\",\n      \"description\": \"Partitioning configuration for the dataset\",\n      \"properties\": {\n        \"dimensions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": {\n                \"type\": \"string\",\n                \"description\": \"Partition dimension name\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"enum\": [\"value\", \"time\"],\n                \"description\": \"Partition dimension type\"\n              },\n              \"params\": {\n                \"type\": \"object\",\n                \"description\": \"Dimension-specific parameters\",\n                \"properties\": {\n                  \"period\": {\n  \
  \                  \"type\": \"string\",\n                    \"enum\": [\"YEAR\", \"MONTH\", \"DAY\", \"HOUR\"],\n                    \"description\": \"Time period for time-based partitions\"\n                  }\n                }\n              }\n            }\n          },\n          \"description\": \"Partition dimensions\"\n        },\n        \"filePathPattern\": {\n          \"type\": \"string\",\n          \"description\": \"File path pattern for file-based partitioned datasets\"\n        }\n      }\n    },\n    \"MetricsSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Metrics computation settings\",\n      \"properties\": {\n        \"probes\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"Metric probe type\"\n              },\n              \"enabled\": {\n                \"type\"\
  : \"boolean\",\n                \"description\": \"Whether this probe is enabled\"\n              },\n              \"computeOnBuildMode\": {\n                \"type\": \"string\",\n                \"enum\": [\"NO\", \"PARTITION\", \"WHOLE_DATASET\"],\n                \"description\": \"When to compute the metric during builds\"\n              }\n            }\n          }\n        },\n        \"displayedState\": {\n          \"type\": \"object\",\n          \"description\": \"Display state for metrics\"\n        }\n      }\n    },\n    \"ChecksSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Data quality check settings\",\n      \"properties\": {\n        \"checks\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"Check type\"\n              },\n              \"name\": {\n                \"\
  type\": \"string\",\n                \"description\": \"Check name\"\n              },\n              \"meta\": {\n                \"type\": \"object\",\n                \"description\": \"Check metadata\"\n              },\n              \"params\": {\n                \"type\": \"object\",\n                \"description\": \"Check parameters\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"VersionTag\": {\n      \"type\": \"object\",\n      \"description\": \"Version tracking information\",\n      \"properties\": {\n        \"versionNumber\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"Sequential version number\"\n        },\n        \"lastModifiedBy\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"login\": {\n              \"type\": \"string\",\n              \"description\": \"Login of the user who made the modification\"\n            }\n          }\n        },\n      \
  \  \"lastModifiedOn\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"description\": \"Timestamp of the last modification\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dataiku/refs/heads/main/json-schema/dataiku-dataset-schema.json
tags:
- Analytics
- Artificial Intelligence
- Data Platform
- Data Science
- Machine Learning
title: Dataiku DSS Dataset
---
