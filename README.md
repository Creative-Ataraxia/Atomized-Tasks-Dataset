## Atomized Tasks Dataset

### Overview

**Atomized Tasks Dataset** is a tabular dataset of 6,970 real-world automation templates; These workflows are commonly used in SaaS, e-commerce, advertising, marketing, sales, customer support, etc. Each row represents an *atomic task*: a minimal, reusable workflow component within a larger business process.

This dataset contains enriched metadata designed to support analysis, research, automation design, and *generating ideas for SaaS products* and AI agent-based tools.

The dataset aims to help solopreneurs, data engineers, automation engineers, and tool builders to explore the underlying 'Lego blocks' of real-world business processes, components that are typically opaque to outsiders. By examining how tasks are automated across platforms like Google Sheets, Drive, Notion, Slack, Telegram, Airtable, etc., and how generative AI models like ChatGPT, Claude, and Gemini are integrated.

### Dataset Overview

Each row in the dataset describes an individual workflow, and includes the following fields:

| Field         | Description | Data_Type |
|---------------|-------------| --------- |
| `title`       | Title of the workflow | String |
| `source`      | The source system(s) where data originates | String |
| `target`      | The target system(s) where data is sent or written to | String |
| `action`      | Primary data engineering action of the workflow | String |
| `action_full` | A concise explanation describing what the task does | String |
| `DE_part`     | Technical summary using data engineering terms | String |
| `is_big_data` | Does the workflow likely involves data streaming or frequent data updates | Boolean |
| `is_LLM`      | Does the workflow involves a generative AI model | Boolean |

### Repo Structure

```ascii
atomized-tasks/
├── CSVs/
│   ├── merged_part_1.csv        # Main dataset chunks in csv format; Each csv chunk contains 500 workflows
│   ├── merged_part_2.csv
│   ├── merged_part_3.csv
│   ├── merged_part_4.csv
│   └── merged_part_5.csv
│   ...
├── Excels/
│   ├── merged_part_1.xlsx       # dataset chunks in excel spreadsheet format, for easy downloading and usage
│   ├── merged_part_2.xlsx
│   ├── merged_part_3.xlsx
│   ├── merged_part_4.xlsx
│   └── merged_part_5.xlsx
│   ...
├── README.md                    # Readme file of this repo
└── LICENSE                      # license file
```

### Possible Uses

* As reference dataset for designing AI agent workflows
* Find ideas for building and launching micro SaaS tools
* Find micro-automation services opportunities for consulting or resale
* Analyze common automation patterns and build visualizations for research papers
* Explore UX patterns for workflow builders or SaaS integrations
...


### Quickstart

> For quick browsing, download the excel spreadsheet of the dataset chunks

Recommend using your favorite EDA tool for more in-depth explorations: `pandas`, `polars`, `spark`


### Contacts for Services

Please reach out to me (roy.ma9@gmail.com)[roy.ma9@gmail.com] if you have any questions regarding this dataset, or if you want to work with me to implement any workflows for your company or use cases.


### License

This dataset is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
You are free to use, adapt, and build upon the dataset — including for commercial use — **as long as you provide proper attribution**.  
Please credit: **Creative-Ataraxia (https://github.com/Creative-Ataraxia)** or link back to this repository.
