# Awesome MCP Security [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curation of awesome resources, papers, and tools focused on Model Context Protocol (MCP) security.

Contributions are always welcome. Please read the [Contribution Guidelines](CONTRIBUTING.md) before contributing.

## Table of Contents

- [Awesome MCP Security](#awesome-mcp-security)
  - [Table of Contents](#table-of-contents)
  - [Papers](#papers)
  - [Security Vulnerabilities](#security-vulnerabilities)
  - [Tools](#tools)
  - [Articles and Blog Posts](#articles-and-blog-posts)
  - [Other Awesome Projects](#other-awesome-projects)
  - [Other Useful Resources](#other-useful-resources)

## Papers

- "Model Context Protocol (MCP): Landscape, Security Threats, and Future Research Directions", 2025-03, [paper](https://arxiv.org/abs/2503.23278)
- "MCP Safety Audit: LLMs with the Model Context Protocol Allow Major Security Exploits", 2025-04, [paper](https://arxiv.org/abs/2504.03767)
- "Enterprise-Grade Security for the Model Context Protocol (MCP): Frameworks and Mitigation Strategies",2025-04, [paper](https://arxiv.org/pdf/2504.08623)

## Security Vulnerabilities

### Authentication and Authorization

- **OAuth Token Theft**: MCP servers store authentication tokens for various services, creating a high-value target for attackers ([Pillar Security](https://www.pillar.security/blog/the-security-risks-of-model-context-protocol-mcp))
- **Permission Boundary Problems**: Unclear boundaries between services connected through MCP ([Block InfoSec](https://block.github.io/goose/blog/2025/03/31/securing-mcp/))

### Prompt Injection

- **Tool Description Manipulation**: Hidden instructions in tool descriptions can cause AI models to perform unauthorized actions ([Pillar Security](https://www.pillar.security/blog/the-security-risks-of-model-context-protocol-mcp))
- **Indirect Prompt Injection**: Malicious content embedded in processed documents that trigger MCP actions ([Pillar Security](https://www.pillar.security/blog/the-security-risks-of-model-context-protocol-mcp))

### Supply Chain

- **Installer Risks**: MCP server installers without proper validation can introduce security risks ([arxiv:2503.23278](https://arxiv.org/abs/2503.23278))
- **Tool Name Conflicts**: Naming collisions in MCP tools can lead to confusion and security issues ([arxiv:2503.23278](https://arxiv.org/abs/2503.23278))

## Tools

- [MCP Specification](https://spec.modelcontextprotocol.io/specification/2025-03-26/) - Official MCP specification with security recommendations
- [Glama.ai MCP Server Directory](https://block.github.io/goose/blog/2025/03/26/mcp-security/) - Security-aware directory of MCP servers with security scoring
- [Damn Vulnerable MCP Server](https://github.com/harishsg993010/damn-vulnerable-MCP-server) - A server intentionally designed with flaws for security testing and training.
- [MCP-scan](https://github.com/invariantlabs-ai/mcp-scan?tab=readme-ov-file) - Security scanning tool designed to go over your installed MCP servers and check them for common security vulnerabilities like prompt injections, tool poisoning and cross-origin escalations.
- [ToolHive](https://github.com/StacklokLabs/toolhive) - Lightweight utility designed to simplify the deployment and management of MCP servers, ensuring ease of use, consistency, and security.
- [MCP-Shield](https://github.com/riseandignite/mcp-shield) - Scans your installed MCP servers and detects vulnerabilities like tool poisoning attacks, exfiltration channels and cross-origin escalations.
- [mcp-injection-experiments](https://github.com/invariantlabs-ai/mcp-injection-experiments/tree/main) - MCP Tool Poisoning Experiments
- [MCP Guardian](https://github.com/eqtylab/mcp-guardian) - Manages your LLM assistant's access to MCP servers, handing you realtime control of your LLM's activity.

## Articles and Blog Posts - 

- [The Security Risks of Model Context Protocol (MCP)](https://www.pillar.security/blog/the-security-risks-of-model-context-protocol-mcp) - Analysis of OAuth token theft and prompt injection risks
- [Securing the Model Context Protocol](https://block.github.io/goose/blog/2025/03/31/securing-mcp/) - Best practices for MCP security by Block's InfoSec team
- [How to Determine If An MCP Server Is Safe](https://block.github.io/goose/blog/2025/03/26/mcp-security/) - Guidelines for evaluating MCP server security
- [AI Model Context Protocol (MCP) and Security](https://community.cisco.com/t5/security-blogs/ai-model-context-protocol-mcp-and-security/ba-p/5274394) - Comprehensive guide by Omar Santos covering MCP security architecture, authentication best practices, data security, and tool exposure security considerations
- [AI agent identity: it's just OAuth](https://mayakaczorowski.com/blogs/ai-agent-authentication) - Discussion about Authentication for AI Agents. Mentions OAuth Fails for MCP based AI Agents.
- [Model Context Protocol has prompt injection security problems](https://simonwillison.net/2025/Apr/9/mcp-prompt-injection/) - As more people start hacking around with implementations of MCP (the Model Context Protocol, a new standard for making tools available to LLM-powered systems) the security implications of tools built on that protocol are starting to come into focus.

## Other Awesome Projects

- [Awesome LLM Security](https://github.com/corca-ai/awesome-llm-security) - A curated list focused on LLM security more broadly
- [Model Context Protocol](https://github.com/modelcontextprotocol) - Official MCP GitHub organization with specification and reference implementations

## Other Useful Resources

- [tl;dr sec #272](https://tldrsec.com/p/tldr-sec-272) - Newsletter discussing AI Model Context Protocol Security
- [tl;dr sec #273](https://tldrsec.com/p/tldr-sec-273) - Newsletter covering MCP security tools and threats
