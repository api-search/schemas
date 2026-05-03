---
description: Schema for a CRAN R package metadata record as returned by the METACRAN CranDB API
layout: schema
name: CRAN Package
properties_list:
- description: Package name on CRAN
  name: Package
  type: string
- description: Current package version using semantic versioning
  name: Version
  type: string
- description: Short one-line title for the package
  name: Title
  type: string
- description: Full package description paragraph
  name: Description
  type: string
- description: Package authors, often in Authors@R format
  name: Author
  type: string
- description: Package maintainer name and email
  name: Maintainer
  type: string
- description: SPDX license identifier
  name: License
  type: string
- description: Required R version and dependent packages
  name: Depends
  type: string
- description: Imported packages required at runtime
  name: Imports
  type: string
- description: Optionally suggested packages
  name: Suggests
  type: string
- description: Packages enhanced by this package
  name: Enhances
  type: string
- description: Package release date
  name: Date
  type: string
- description: URL for the package homepage or development repository
  name: URL
  type: string
- description: URL for submitting bug reports
  name: BugReports
  type: string
- description: Whether the package requires compilation
  name: NeedsCompilation
  type: string
- description: External system requirements for the package
  name: SystemRequirements
  type: string
- description: Repository name (typically CRAN)
  name: Repository
  type: string
- description: CRAN publication timestamp
  name: Date/Publication
  type: string
provider_name: R
provider_slug: r
schema_file: json-schema/r-cran-package-schema.json
slug: r-cran-package
source_filename: r-cran-package-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/json-schema/r-cran-package-schema.json\",\n  \"title\": \"CRAN Package\",\n  \"description\": \"Schema for a CRAN R package metadata record as returned by the METACRAN CranDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Package\": {\n      \"type\": \"string\",\n      \"description\": \"Package name on CRAN\",\n      \"example\": \"ggplot2\"\n    },\n    \"Version\": {\n      \"type\": \"string\",\n      \"description\": \"Current package version using semantic versioning\",\n      \"example\": \"3.4.4\"\n    },\n    \"Title\": {\n      \"type\": \"string\",\n      \"description\": \"Short one-line title for the package\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"Full package description paragraph\"\n    },\n    \"Author\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"Package authors, often in Authors@R format\"\n    },\n    \"Maintainer\": {\n      \"type\": \"string\",\n      \"description\": \"Package maintainer name and email\",\n      \"example\": \"Hadley Wickham <hadley@posit.co>\"\n    },\n    \"License\": {\n      \"type\": \"string\",\n      \"description\": \"SPDX license identifier\",\n      \"example\": \"MIT + file LICENSE\"\n    },\n    \"Depends\": {\n      \"type\": \"string\",\n      \"description\": \"Required R version and dependent packages\"\n    },\n    \"Imports\": {\n      \"type\": \"string\",\n      \"description\": \"Imported packages required at runtime\"\n    },\n    \"Suggests\": {\n      \"type\": \"string\",\n      \"description\": \"Optionally suggested packages\"\n    },\n    \"Enhances\": {\n      \"type\": \"string\",\n      \"description\": \"Packages enhanced by this package\"\n    },\n    \"Date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Package release date\"\n\
  \    },\n    \"URL\": {\n      \"type\": \"string\",\n      \"description\": \"URL for the package homepage or development repository\"\n    },\n    \"BugReports\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL for submitting bug reports\"\n    },\n    \"NeedsCompilation\": {\n      \"type\": \"string\",\n      \"enum\": [\"yes\", \"no\"],\n      \"description\": \"Whether the package requires compilation\"\n    },\n    \"SystemRequirements\": {\n      \"type\": \"string\",\n      \"description\": \"External system requirements for the package\"\n    },\n    \"Repository\": {\n      \"type\": \"string\",\n      \"description\": \"Repository name (typically CRAN)\"\n    },\n    \"Date/Publication\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"CRAN publication timestamp\"\n    }\n  },\n  \"required\": [\"Package\", \"Version\", \"Title\", \"Description\", \"Maintainer\", \"License\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/r/refs/heads/main/json-schema/r-cran-package-schema.json
tags:
- R
- Statistics
- Data Science
- Open Source
- Programming Language
title: CRAN Package
---
