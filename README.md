# Cams_Online-assesment
Senior AI Applications Engineer

The deliverables are as follows:

1. CamsAI_Invoice_Auditor_Source_Code.zip — Full source code including the LangGraph multi-agent orchestrator, FastAPI MCP server with all 5 APIs, Docker Compose stack, ChromaDB vector knowledge base, PostgreSQL ledger, and Slack escalation integration.

2. CamsAI_Invoice_Auditor_System_Design.pdf — System design document covering the solution architecture, state machine design, agent responsibilities, governance, observability strategy, and production scaling plan.

3. CamsAI_Invoice_Audit_Log_Output.csv — Live audit log output from the pipeline run, showing 196 unique invoices processed across 3 mock scenarios and 123 real invoice images sourced from the Voxel51 and mychen76 HuggingFace datasets. Each row captures the timestamp, vendor, total amount, compliance score, decision, anomaly flags, and ledger or alert ID.

The pipeline is designed to run continuously across the full datasets — 8,181 images from Voxel51 and 1,489 from mychen76 — without any code changes. The output has been limited to the current sample size purely for demonstration and API cost purposes. The sample count can be scaled to the full dataset by updating two environment variables (VOXEL51_SAMPLES and MYCHEN76_SAMPLES) before running.

The system can be run end-to-end with a single command:
docker-compose up --build
Having updated ANTHROPIC_API_KEY and HF_TOKEN. 

Best regards,
Shiva Prasaath
