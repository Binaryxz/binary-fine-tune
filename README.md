
WebTorrent
The no-code platform for building custom LLM Agents

📄 Documentation
Features
Load data from anywhere
Raw text
Web page
Files
Word
Excel
Powerpoint
PDF
Markdown
Plain Text
Web Site (coming soon)
Notion (coming soon)
Airtable (coming soon)
No-code: User-friendly interface to manage your datastores and chat with your data
Securized API endpoint for querying your data
Auto sync data sources (coming soon)
Auto generates a ChatGPT Plugin for each datastore
Semantic Search Specs
Vector Datbase: Qdrant
Embeddigs: Openai's text-embedding-ada-002
Chunk size: 256 tokens
Stack
Next.js
Joy UI
LangchainJS
PostgreSQL
Prisma
Qdrant
Inspired by the ChatGPT Retrieval Plugin.

Run the project locally
Without docker compose
Minimum requirements to run the projects locally

Node.js v18
Postgres Database
Redis
Qdrant
GitHub App (NextAuth)
Email Provider (NextAuth)
OpenAI API Key
AWS S3 Credentials
Run locally (Docker)
cp .dev/databerry/app.env.example .dev/databerry/app.env
# Add your own OPENAI_API_KEY

-------------------------------------

pnpm docker:compose up

# Alternatively run app and services separately
pnpm docker:compose:deps up
pnpm docker:compose:app up

# create s3 bucket
# go to http://localhost:9090 and create bucket databerry-dev
# set bucket access policy to public
# might need to add 127.0.0.1 minio to /etc/hosts in order to access public s3 files through http://minio...

# Dev emails inbox (maildev)
# visit http://localhost:1080

You can fully rebuild dockers with :
pnpm docker:compose up --build





