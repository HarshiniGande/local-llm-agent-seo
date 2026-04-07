# Local LLM Agent for Automated SEO Content Workflow

Autonomous AI agent running on local hardware, integrated with the Claude API via MCP to automate a multi-step SEO content pipeline.

## Stack
Python · Ollama · Mistral 7B · Claude API · MCP (Model Context Protocol) · Bash

## What it does
- Deploys Mistral 7B locally via Ollama on a Linux machine
- Orchestrates a multi-step agent workflow: ingests keyword briefs, generates draft content, routes outputs to structured folders
- Integrates Claude API via MCP for final generation, leveraging its stronger instruction-following for tone and nuance
- Python and Bash scripts handle model serving, failure monitoring, and output logging

## Key result
Reduced a 3-hour manual content workflow to under 12 minutes end-to-end.

## Infrastructure notes
- Model serving monitored via latency logging; failures trigger automatic restart
- All infrastructure decisions documented in operational runbook
- Designed for reproducibility — configuration files version-controlled alongside code
