# AI Call Summaries - Implementation Brief

**Date:** May 2025 | **Participant:** Brittany Ho (Client Experience)

## Executive Summary

Discovery call with Brittany went well - requirements are clear, specific, and immediately actionable. Three core deliverables identified: (1) automated call summaries with bullet-point topics, (2) positive/negative sentiment analysis with defined trigger phrases (captured verbatim from Brittany), and (3) upsell opportunity detection based on performance/budget indicators.

**What I need from you:** API access for Fireflies and Slack integrations to start V1. (I'll send clear instructions or hop on a quick call to walk through this - won't be complicated.)

**Timeline:** V1 (summaries + Slack) ready in 2-3 days of receiving access. V2 (task automation) after feedback and iteration on summary quality.

**Pilot:** Starting with Solgaard (multiple weekly calls, high visibility).

**Context:** This implements the call summary automation component of the AI audit initiative.

## Technical Specifications & Requirements

### Pilot Client

**Solgaard** (luggage company) - Multiple weekly calls across channels

### Core Deliverables

**1. High-level summary of what was discussed in the call**

Very succinct bullet points of topics discussed

Auto-posted to client-specific Slack channels

**2. Sentiment Analysis** *(All triggers and phrases below captured directly from Brittany during discovery call)*

**Positive Indicators:**

**Performance-related:** 'great', 'excellent', 'so happy'

**Creative-related:** Compliments on creative work and team output

**Team/individuals:** Recognition and praise for specific team members

**Negative Triggers (High Priority - Creates ClickUp Tasks):**

**Performance down:** 'Why is performance down?' frustration, upset, 'Why haven't you communicated major optimizations to the team prior?', 'Why weren't you pro-active?'

**Timeliness:** 'Why is this taking so long?', 'Why is this being delayed?', 'How much longer do we have to wait?', 'It's already been [timeline]?'

**Campaigns/evergreen/aligning on strategy:** 'No approvals yet…'

**3. Upsell Opportunity Detection** Identify opportunities already starting:

'We're scaling well on paid social…'

'We have more budget…'

'Talking about a different platform'

'We need more creative…'

If client using only one service (expansion opportunity)

Performance indicators showing strength

### Key Contacts (Solgaard)

Luke, Haily, Chris, Adrian (CEO), Kelsey

### Integration Requirements

**Fireflies API:** Access to call transcripts

**Slack API:** Auto-posting summaries to client channels

**ClickUp API:** Task creation for negative sentiment alerts

### Goal

Grow account through proactive client management and systematic upsell identification.
