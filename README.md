# Sub-Agents Setup Guide for Claude Code

As we are fans of building agent systems, we couldn't pass by helping those who need help setting up agents in Claude Code.

## 📁 File Structure

Create the following structure in your project:

```
your-project/
├── .claude/
│   └── agents/
│       ├── reddit-intelligence.md
│       ├── tam-market-size.md
│       ├── competitive-intelligence.md
│       ├── business-model.md
│       ├── supabase-specialist.md
│       ├── performance-optimizer.md
│       ├── seo-specialist.md
│       ├── security-auditor.md
│       └── qa-engineer.md
```

## 🚀 Quick Setup

### Step 1: Create agents folder
```bash
mkdir -p .claude/agents
```

### Step 2: Create agent files

For each agent:
1. Create a file named: `agent-name.md`
2. Copy **only** the content between `---` (YAML header) and the entire System Prompt
3. DO NOT copy instructions, usage examples, or other guide sections

### What to copy from each file:

#### Example structure (DO NOT copy this example, it's just a template):
```markdown
---
name: agent-name
description: MUST BE USED PROACTIVELY...
tools: web_search, web_fetch, repl
---

# Agent Name System Prompt

You are an expert specializing in...

[All remaining System Prompt content]
```

## 📋 Complete Agent List

### Business Research Agents:

1. **reddit-intelligence.md**
   - Search and analyze Reddit discussions
   - Extract insights and trends
   - Identify pain points and opportunities

2. **tam-market-size.md**
   - Calculate market size (TAM/SAM/SOM)
   - Analyze market opportunities
   - Industry research and sizing

3. **competitive-intelligence.md**
   - Analyze competitors
   - Find market gaps
   - Strategic positioning research

4. **business-model.md**
   - Research monetization strategies
   - Analyze business models
   - Unit economics evaluation

### Technical Agents:

5. **supabase-specialist.md**
   - Supabase security setup
   - Realtime, Edge Functions, Cron
   - RLS policies and auth

6. **performance-optimizer.md**
   - Node.js/React optimization
   - Performance improvements
   - Bundle size reduction

7. **seo-specialist.md**
   - SEO optimization
   - Schema.org markup
   - Search engine optimization

8. **security-auditor.md**
   - Security audits
   - Vulnerability detection
   - OWASP compliance

9. **qa-engineer.md**
   - Test automation
   - Quality assurance
   - E2E, unit, integration testing

## 💡 How to Use Agents

### Automatic Usage:
Claude will automatically select the appropriate agent based on your request:
```
"Find discussions about e-scooters on Reddit"
"What's the market size for SaaS CRM?"
"Set up security in Supabase"
```

### Explicit Agent Call:
Specify a particular agent:
```
"Use reddit-intelligence to analyze reviews"
"Apply seo-specialist to optimize the homepage"
```

## 🔧 Verify Installation

1. Open terminal in project root
2. Type command: `/agents`
3. You should see all 9 agents listed

## ❓ Frequently Asked Questions

**Q: Should I copy all code examples?**
A: Yes, copy the entire System Prompt including code examples - this helps the agent work correctly.

**Q: Can I modify agent descriptions?**
A: Yes, you can adapt descriptions to your needs, but keep key phrases like "MUST BE USED PROACTIVELY".

**Q: How do I add new tools to an agent?**
A: Use the `/agents` command, select the agent, and edit the tools list.

## 📚 Additional Resources

- [Claude Code Documentation](https://docs.anthropic.com/en/docs/claude-code/sub-agents)
- Usage examples are in the full guides for each agent
- For issues, create an issue in your project repository

## ✅ Installation Checklist

- [ ] Created `.claude/agents/` folder
- [ ] Copied all 9 agent files
- [ ] Each file has YAML header and System Prompt
- [ ] Verified via `/agents` command
- [ ] Tested at least one agent

## 🎯 Agent Capabilities Summary

### Business Research:
- **Reddit Intelligence**: Community insights, trend analysis, pain point discovery
- **TAM/Market Size**: Market sizing, growth analysis, opportunity assessment
- **Competitive Intelligence**: Competitor analysis, positioning, differentiation
- **Business Model**: Monetization research, pricing strategy, unit economics

### Technical Excellence:
- **Supabase Specialist**: Auth, RLS, realtime, edge functions, security
- **Performance Optimizer**: Speed optimization, bundle reduction, caching
- **SEO Specialist**: Technical SEO, schema markup, search optimization
- **Security Auditor**: Vulnerability detection, security best practices
- **QA Engineer**: Automated testing, quality assurance, test coverage

## 🚦 Getting Started

1. **Install agents** using this guide
2. **Test with simple requests** to see agents in action
3. **Explore capabilities** by asking complex questions
4. **Customize as needed** for your specific use cases

