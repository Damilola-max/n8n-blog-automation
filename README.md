# n8n Blog Automation System

## Overview
Automates blog publishing pipeline:

Email → Content Processing → WordPress Draft → Jira Review → AI Content → Trello Distribution → Publish

## Features
- Email-triggered automation
- SEO meta generation (Yoast)
- AI social media generation
- Jira approval workflow
- Trello content distribution
- Automated publishing

## Architecture
IMAP → n8n → WordPress → Jira → OpenAI → Trello → Publish

## Setup

### 1. Clone repo
git clone https://github.com/YOUR_USERNAME/n8n-blog-automation.git

### 2. Configure environment
cp credentials/.env.example credentials/.env

### 3. Run system
cd docker
docker-compose up -d

### 4. Open n8n
http://localhost:5678

### 5. Import workflow
Import workflows/blog-automation.json

## Notes
- Configure credentials manually inside n8n UI
- Do NOT commit secrets
