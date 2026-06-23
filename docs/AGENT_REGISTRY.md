# Agent Registry — All Agents + Prompts

## 1. Shadow Clone Agent
Path: agents/shadow-clone-agent/
Trigger: New client URL submitted
Sub-agents: 10 (asyncio.gather)
Output: MANIFEST.json, full clone, API map

## 2. QA Agent (EXTREMELY PICKY)
Path: agents/qa-agent/
Trigger: Every build completion
Threshold: 100% across all 10 categories
Output: QA report, per-failure line numbers + fixes

## 3. Security Agent
Path: agents/security-agent/
Trigger: Every 5 minutes (cron) + on clone
Patterns: 35 key/secret types
Output: Risk score, grade, remediation

## 4. AI Enhancement Agent
Path: agents/ai-enhancement-agent/
Trigger: After clone complete
Output: Ranked recommendations, market value, proposal

## 5. Headless Operator Agent
Path: agents/headless-operator-agent/
Trigger: After every build in sandbox
Loop: Builds until QA scores 100%
Output: Test results, screenshots, score

## 6. Audit Agent
Path: agents/audit-agent/
Trigger: After discovery
Output: Content audit, image audit, performance audit

## 7. Chat Moderator Agent
Path: agents/chat-moderator-agent/
Trigger: Client message in dashboard
Output: Automated response or escalation

## 8. SEO Intelligence Agent
Path: agents/seo-agent/
Trigger: Every hour (cron)
Output: Rankings, keyword harvest, competitor data

## 9. Social Media Agent
Path: agents/social-media-agent/
Trigger: Daily (cron)
Platforms: Instagram, YouTube, TikTok, Facebook, LinkedIn, Twitter, Pinterest, Reddit
Output: Leads, hashtags, top content

## 10. Backend Cloner Agent
Path: agents/backend-cloner/
Trigger: On shadow clone run
Output: DB schema, API map, auth flows, webhooks
