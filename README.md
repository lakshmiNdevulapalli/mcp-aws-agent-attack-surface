# MCP-Enabled AI Agent Attack Surface Analysis in AWS

## Overview 

This repository contains research artifacts, experimental notes, and supporting materials for an independent study on the security implications of Model Context Protocol (MCP)–enabled AI agents operating in Amazon Web Services (AWS) cloud environments.

The research investigates how autonomous AI agents with tool-use capabilities introduce novel attack surfaces that are not adequately addressed by existing cloud security threat models.

**Status:** Private research repository  
**Intended publication:** IEEE (security/cloud systems track)

## Research Objectives

The primary objectives of this research are:

- Identify and characterize new attack vectors introduced by MCP-enabled AI agents in cloud environments
- Develop a threat taxonomy for MCP-mediated cloud attacks
- Empirically validate attack feasibility through controlled red-team exercises
- Analyze detection gaps in existing AWS security tooling (CloudTrail, GuardDuty)
- Propose behavior-based detection signatures for AI-initiated attacks

## Research Questions

This study is guided by the following research questions:

- RQ1: What novel attack vectors emerge when AI agents with MCP tool access operate within AWS cloud environments, and how do these differ from traditional cloud security threats?
- RQ2:	How can prompt injection attacks be chained through MCP tool calls to achieve unauthorized access to cloud resources (IAM, Lambda, S3, Secrets Manager)?
- RQ3:	What is the prevalence of exploitable vulnerabilities in open-source MCP server implementations when deployed in production cloud environments?
- RQ4:	What detection signatures and monitoring strategies can identify MCP-based attacks in AWS CloudTrail logs and GuardDuty findings?
- RQ5:	What architectural patterns and security controls effectively mitigate MCP-cloud attack vectors while preserving agent functionality?

## Methodology

The research methodology combines:

- Static analysis of publicly available MCP server implementations
- Dynamic red-team testing on production-representative AWS environments
- Controlled proof-of-concept attack development targeting:
  - AWS IAM
  - AWS Lambda
  - Amazon S3
  - AWS Secrets Manager
- Analysis of cloud audit and detection logs to derive observable attack signatures

All experiments are conducted using self-funded, non-production AWS accounts with no access to proprietary datasets or enterprise systems.

## Publication Plan

The findings from this repository are intended for submission to an IEEE conference or journal. Preprint publication may follow formal submission in accordance with IEEE policies.

## License

All rights reserved.
Copyright © 2025 Lakshmi Narasimha, Devulapalli Venkata

This repository and its contents are proprietary and confidential.
Unauthorized copying, distribution, or reuse is prohibited.
