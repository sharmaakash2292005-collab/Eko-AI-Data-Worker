# Eko AI-Assisted Data Worker

An AI-assisted Data Worker prototype designed to analyze partner business performance, identify partners requiring attention, prioritize them, recommend actions, and validate data before automated recommendations proceed.

## Project Objective

The goal is to reduce manual effort in partner performance analysis by converting business data into structured, action-oriented outputs.

## Workflow

Input Data  
→ Data Analysis  
→ Classification  
→ Priority  
→ Action Recommendation  
→ Validation  
→ Human Review / Output

## Project Components

- Power BI dashboard
- Sample business dataset
- Partner classification and prioritization
- Action recommendations
- Validation and exception workflow
- Human-review escalation
- Project documentation

## Repository Structure

```text
Eko-AI-Data-Worker/
│
├── data/
│   └── Akash_Sharma_Eko_AI_Data_Worker_Sample_Dataset.xlsx
│
├── powerbi/
│   └── Akash_Sharma_Eko_AI_Data_Worker.pbix
│
├── documentation/
│   └── Eko_AI_Data_Worker_Documentation.pdf
│
└── README.md
```

## Current Version

The current prototype uses rule-based decision logic implemented through Power BI/DAX for explainable and auditable outputs.

The workflow analyzes partner performance, assigns classifications and priorities, recommends actions, and validates records before allowing the output to proceed.

## Intentional Failure Scenario

The project includes an intentional missing-data scenario for partner EKO10250.

The validation layer detects the missing GMV Growth input and changes the record status to "Requires Human Review" instead of allowing the recommendation to proceed automatically.

## Demo

The project demo video is available in the accompanying Google Drive submission folder.

https://drive.google.com/drive/folders/1Mgd-Mb4gw8vT-ENcim_84-tc4wq8ot4X?usp=sharing

## Future Improvements

The next version could introduce an LLM layer for contextual recommendations, anomaly explanations, and workflow automation while retaining deterministic validation and human-review controls.
