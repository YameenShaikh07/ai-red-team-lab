# AI Red Team Lab - LLM Prompt Injection Attack

A security research project testing prompt injection vulnerabilities in open-source LLMs.

## Overview

This lab demonstrates common prompt injection attacks against TinyLlama and documents how safety guardrails can be bypassed through various techniques including:

- DAN (Do Anything Now) jailbreak
- Fictional framing attacks
- Role-play persona injection
- Instruction override attempts
- Token smuggling

## Results

5 payloads tested. All produced responses indicating guardrail vulnerabilities.

**Critical Finding:** Fictional framing successfully bypassed safety filters and produced restricted content.

## Setup

```bash
python3 -m venv venv
source venv/bin/activate
pip install ollama
ollama pull tinyllama
python scripts/prompt_injection_test.py
```

## Files

- `scripts/prompt_injection_test.py` - Main attack automation scripts
- `results/test_results.json` - Attack results and model responses
- `findings-report.md` - Detailed findings and severity analysis

## Author

Yameen Shaikh| AI Security Researcher | Penetration Tester | Security Analyst

## Disclaimer

For educational and authorized security testing only.
