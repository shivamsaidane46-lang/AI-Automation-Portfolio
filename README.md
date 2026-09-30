# AI Automation Portfolio

Six n8n workflow systems demonstrating AI-assisted business automation, integrations, deterministic routing, validation, reporting, monitoring, and human-in-the-loop escalation.

> **Security:** These workflow exports are sanitized for public sharing. n8n credential objects and webhook identifiers have been removed. Environment-specific resource IDs and URLs are replaced with placeholders where applicable. Configure your own credentials and resource IDs after import.

## Workflows

### 1. Automated Multi-Channel Social & Video Content Repurposer
`workflows/01-social-video-content-repurposer/workflow.json`

Repurposes uploaded long-form audio/video into structured LinkedIn and X/Twitter content and stores the review-ready output in Airtable.

### 2. Automated Weekly Executive Business Health Digest
`workflows/02-weekly-executive-business-health-digest/workflow.json`

Aggregates weekly payment, advertising, and CRM metrics, calculates trends, generates an executive report, and delivers it to leadership.

### 3. Autonomous Customer Onboarding Concierge
`workflows/03-customer-onboarding-concierge/workflow.json`

Turns successful payment or signed-proposal events into a deduplicated client onboarding process with automated workspace provisioning and notifications.

### 4. Competitor Price & Inventory Tracking Sentinel
`workflows/04-competitor-price-inventory-sentinel/workflow.json`

Monitors competitor product pages, normalizes pricing and stock data, detects meaningful changes, and alerts the team.

### 5. Multi-Format Accounts Payable & Invoice Extraction Pipeline
`workflows/05-accounts-payable-invoice-extraction/workflow.json`

Extracts structured invoice data from PDFs/images, validates totals and required fields, and routes exceptions for human review.

### 6. Omnichannel Support Ticket Triage & Smart Escalation
`workflows/06-omnichannel-support-triage/workflow.json`

Combines email/chat intake, knowledge retrieval, sentiment analysis, deterministic routing, AI responses, escalation, logging, and error handling.

## Import

1. Import the relevant `workflow.json` into n8n.
2. Recreate/connect the required credentials in your own n8n instance.
3. Replace placeholders such as `YOUR_AIRTABLE_BASE_ID`, `YOUR_AIRTABLE_TABLE_ID`, `YOUR_GOOGLE_DRIVE_FOLDER_ID`, and `YOUR_SLACK_CHANNEL_ID`.
4. Review webhook paths and external endpoints.
5. Test every branch with non-production data before deployment.

## Security

Never commit API keys, OAuth tokens, passwords, webhook secrets, private database credentials, or production customer data. Use n8n's credential store and environment-specific configuration.

## Status

These are portfolio/demo workflow implementations. Production deployment would require environment-specific configuration, access controls, monitoring, retry/rate-limit handling, privacy review, and additional testing.
