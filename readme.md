# Getting Started

Welcome to your new CAP project.

It contains these folders and files, following our recommended project layout:

File or Folder | Purpose
---------|----------
`app/` | content for UI frontends goes here
`db/` | your domain models and data go here
`srv/` | your service models and code go here
`readme.md` | this getting started guide

## Next Steps

- Open a new terminal and run `cds watch`
- (in VS Code simply choose _**Terminal** > Run Task > cds watch_)
- Start with your domain model, in a CDS file in `db/`

## Learn More

Learn more at <https://cap.cloud.sap>.


https://github.com/SAP-archive/cap-llm-plugin-samples/blob/main/samples/rag-quickstart-app/package.json

https://github.com/SAP-archive/cap-ai-vector-engine-sample/tree/main/application

cf create-service hana hdi-shared capllm-db
cf create-service-key capllm-db capllm-db-key
cds bind -2 capllm-db:capllm-db-key
cds build --production
cds deploy -2 hana:capllm-db

cf create-service destination lite capllm-destination
cf create-service-key capllm-destination capllm-destination-key
destination created aicore-destination.json