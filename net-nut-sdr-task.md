# SDR AI Workflow & Prompting Guide

**Name:** Tomer Berenstein  
**Date:** 13/07/25

---

## 1. Initial Response Draft

### 📝 **PROMPT:**

I'm an SDR at NetNut (proxy company) and received this inbound lead: "Hi, I'm looking for a proxy solution for scraping e-commerce sites in the US and Europe. I need something stable, fast, and ideally with rotating IPs. Can you help?" "Do you have Socks5?" "What is the best tool to scrape Google?"

Help me write a professional email response that:

- Acknowledges their specific requirements (stable, fast, rotating IPs, SOCKS5, Google scraping)
- Highlights NetNut's key differentiators: hybrid network, fastest on market via one-hop ISP connectivity, 91% success rates, zero CAPTCHAs, 24/7 support
- Includes 2-3 qualifying questions about data volume, session needs, and current challenges
- Ends with a clear call-to-action for a 7-day free trial (100GB bandwidth included) - Keep it under 200 words, professional but friendly tone

### 📧 **OUTPUT:**

**Subject: Perfect Proxy Solution for Your E-commerce Scraping Needs**

Hi [Name],

Thanks for reaching out! I can definitely help with your e-commerce scraping requirements in the US and Europe.

NetNut is ideal for your needs. Our hybrid network delivers the fastest speeds on the market through one-hop ISP connectivity, achieving 91% success rates with zero CAPTCHAs. We offer both HTTP and SOCKS5 protocols with automatic IP rotation – perfect for stable, high-performance scraping across all major e-commerce platforms, including Google.

With our 24/7 support team and premium infrastructure, you'll have reliable access to clean residential and datacenter IPs that won't get blocked.

To recommend the optimal setup for you:

- What's your expected monthly data volume?
- Do you need sticky sessions or prefer rapid rotation?
- What challenges are you facing with your current solution?

I'd love to set you up with our 7-day free trial (100GB bandwidth included) so you can test our performance firsthand. Would you be available for a quick 15-minute call this week to discuss your specific requirements and get you started?

Best regards,
[Your Name]
NetNut Proxy Solutions

*Ready to experience zero-downtime scraping? Let's get your trial activated today.*

### 📸 **Screenshots**

![alt text](<Screenshot 2025-07-13 at 15.58.46.png>)

---

## 2. AI Prompting Task

### 🎯 **Prompt 1: Initial Content Creation**

**Prompt Used:**
```
You're helping me craft outreach material for NetNut, a proxy-network provider.

Key points to work in naturally
• Hybrid network: direct ISP IPs + 85 M rotating residential IPs
• One-hop ISP routing → market-leading speed and low latency
• 91% average success, zero CAPTCHAs / IP blocks
• SOCKS5 & HTTP, unlimited concurrency, 24/7 live support
• 7-day free trial with 100 GB bandwidth

Please deliver three clearly labeled items:

1. LinkedIn message – no more than 60 words, professional but friendly, ending with an invitation to a brief call or the free-trial link.

2. One-paragraph product pitch – 90-100 words aimed at teams scraping price and catalog data from US/EU e-commerce sites (Amazon, eBay, etc.).

3. Three discovery questions – concise, covering expected data volume, session/rotation requirements, and current scraping challenges.

Use a confident, helpful tone and weave the key points smoothly into each piece.
```

**Initial AI Output:**
The AI provided technically-focused materials that included detailed specifications and technical language, making them potentially intimidating for prospects.

### 🔄 **Prompt 2: Refinement for Friendliness**

**Prompt Used:**
```
You're just dumping tech on them... This can scare them away. It should be more friendly and inviting.
```

### ✅ **Final AI Output:**

#### 📱 **LinkedIn Message**

Hi [Name], I noticed your team works with e-commerce data collection. We help companies eliminate those frustrating IP blocks and CAPTCHAs that slow down scraping projects. Our clients see 91% success rates and much faster data collection. I'd love to offer you a free 7-day trial with 100GB included – no strings attached. Worth a quick chat?

**Word count: 56 words**

#### 📝 **Product Pitch for E-commerce Scraping Teams**

Tired of constantly hitting blocks and CAPTCHAs when collecting product data from Amazon, eBay, and other major sites? We get it – it's frustrating when your scraping projects get interrupted just when you need fresh pricing or inventory data. NetNut makes this headache disappear with our reliable network that delivers 91% success rates and faster data collection. We combine premium residential IPs with direct connections for speed you can actually feel. Plus, our team provides real human support 24/7 whenever you need help. No more babysitting your scrapers or explaining delays to stakeholders.

**Word count: 97 words**

#### ❓ **Discovery Questions**

1. **Scale**: How much data are you typically collecting each month, and are you looking to expand your coverage?

2. **Workflow**: Do you prefer to stick with the same IP for multi-step processes, or would faster rotation work better for your projects?

3. **Pain Points**: What's your biggest headache right now with data collection – is it blocks, slow speeds, or something else entirely?

### 🚀 **Key Improvements Made by AI**

- **Tone shift**: From technical specifications to empathetic problem-solving
- **Language simplification**: Replaced jargon with conversational terms
- **Benefit-focused**: Emphasized outcomes rather than features
- **Emotional connection**: Acknowledged prospect frustrations and positioned NetNut as the solution

### 📸 **Screenshots**

![alt text](image.png)
![alt text](image-1.png)
---

## 3. SDR AI Automation Workflow - Technical Implementation

### 🔍 **My Prompt Journey**

**First Prompt I Tried:**
"Suggest one practical way I could use AI to streamline my daily SDR workflow. Describe the improvement step by step, including which common systems it would connect to (email, calendar, CRM), and estimate the time saved or lift in response rates. Keep the explanation professional, concise, and under 120 words in length. Try to use an existing AI model or framework I can use."

**Why I Didn't Like It:**
The response was too high-level and didn't give me enough technical detail to actually implement anything.

**Second Prompt That Worked:**
"Need a more detailed workflow that effectively explains how each part is done technically."

**What This Got Me:**
The comprehensive technical implementation guide below that actually shows me how to build this system step by step.

### ⚙️ **What This System Actually Does**

This is an automated research and outreach system that takes the manual grunt work out of SDR prospecting. Here's the simple version:

1. **New lead enters my CRM** → System automatically triggers
2. **AI researches the prospect** → Pulls company data, recent news, LinkedIn activity
3. **AI writes personalized email** → Creates relevant conversation starters based on research
4. **Email gets sent** → Automatically delivered through my existing email platform

Instead of me spending 8-10 minutes manually researching each prospect and writing generic emails, the AI does deep research in 45 seconds and creates highly personalized outreach that gets 2-3x better response rates.

The result: I can process 60-80 prospects per day instead of 15-20, with much better quality and higher response rates.

### 🏗️ **System Architecture Overview**

**Core Components:**
- CRM (Salesforce/HubSpot) - Lead source
- Make.com/Zapier - Orchestration platform
- OpenAI API (GPT-4) or Claude API - AI processing
- Apollo.io/ZoomInfo API - Company data enrichment
- LinkedIn Sales Navigator API - Professional insights
- Email platform (Outreach/SalesLoft) - Delivery system

### 📋 **Step-by-Step Technical Workflow**

#### 1️⃣ **Trigger Setup (Make.com/Zapier)**

```
Trigger: New lead added to CRM or lead status changed to "Research"
Webhook: CRM sends lead data (name, company, title, LinkedIn URL, email)
```

#### 2️⃣ **Data Enrichment Phase**

**Apollo.io API Call:**
```javascript
GET https://api.apollo.io/v1/people/match
Headers:
- X-Api-Key: YOUR_API_KEY
Payload: {
"first_name": "John",
"last_name": "Smith",
"organization_name": "TechCorp Inc",
"email": "john@techcorp.com"
}
```

**Response extracts:**
- Company size, industry, recent funding
- Technologies used
- Recent news/press releases
- Contact's job tenure and background

#### 3️⃣ **LinkedIn Intelligence Gathering**

**LinkedIn Sales Navigator API:**
```javascript
GET https://api.linkedin.com/v2/people/{person-id}
Headers:
- Authorization: Bearer LINKEDIN_TOKEN
```

**Captures:**
- Recent posts and activity
- Shared connections
- Company updates and job changes
- Professional achievements

#### 4️⃣ **AI Research Processing**

**OpenAI API Call Structure:**
```javascript
POST https://api.openai.com/v1/chat/completions
Headers:
- Authorization: Bearer OPENAI_API_KEY
- Content-Type: application/json

Payload: {
"model": "gpt-4",
"messages": [
{
"role": "system",
"content": "You are an expert SDR researcher. Analyze prospect data and create personalized outreach insights."
},
{
"role": "user",
"content": "Prospect: John Smith, VP Sales at TechCorp Inc. Company data: [enriched_data]. LinkedIn activity: [linkedin_insights]. Create 3 personalized conversation starters and identify key pain points."
}
],
"max_tokens": 500
}
```

**AI Output Format:**
```json
{
"conversation_starters": [
"Saw TechCorp's recent Series B announcement - congrats! Are you scaling the sales team with the new funding?",
"Notice you've been hiring SDRs lately. What's been your biggest challenge with sales development?",
"Your recent LinkedIn post about sales automation resonated with me..."
],
"pain_points": ["Scaling challenges", "Lead quality", "Sales process efficiency"],
"personalization_notes": "Recent promotion, company growth phase, active on LinkedIn"
}
```

#### 5️⃣ **Email Template Generation**

**Second AI API Call:**
```javascript
"content": "Using these insights: [ai_research_output], write a personalized cold email for [prospect_name] at [company]. Use conversation starter #1. Keep it under 100 words, professional tone, include clear CTA."
```

**Generated Email Structure:**
```
Subject: Quick question about TechCorp's sales expansion

Hi John,

Saw TechCorp's recent Series B announcement - congrats!

I imagine you're scaling the sales team with the new funding. I work with VP Sales at similar growth-stage companies who are facing challenges with lead qualification and rep productivity during rapid scaling.

Would you be open to a brief 15-minute call this week to discuss how [Your Company] helped [Similar Company] increase qualified leads by 40% during their expansion?

Best,
[Your Name]
```

#### 6️⃣ **CRM Integration & Email Delivery**

**Salesforce API Update:**
```javascript
POST https://[instance].salesforce.com/services/data/v54.0/sobjects/Lead/[lead_id]
Headers:
- Authorization: Bearer SALESFORCE_TOKEN
Payload: {
"Research_Notes__c": "[AI generated insights]",
"Personalization_Angle__c": "[conversation_starter_used]",
"Outreach_Status__c": "Email Generated"
}
```

**Outreach.io API Integration:**
```javascript
POST https://api.outreach.io/api/v2/mailings
Headers:
- Authorization: Bearer OUTREACH_TOKEN
Payload: {
"data": {
"type": "mailing",
"attributes": {
"subject": "[generated_subject]",
"bodyText": "[generated_email]",
"mailboxId": YOUR_MAILBOX_ID
},
"relationships": {
"prospect": {
"data": {"type": "prospect", "id": prospect_id}
}
}
}
}
```

### 🎯 **Why This Will Transform My SDR Performance**

**Better Research:** I'll get way deeper insights like funding rounds, tech stack changes, and timing signals that I'd never find manually. This gives me actual conversation starters and real pain points to reference instead of generic stuff.

**Messages That Actually Work:** Instead of boring templates, I'll send super relevant outreach that mentions specific company events and challenges. My response rates will jump big time.

**Totally Different Daily Routine:** I'll go from spending 2-3 hours researching 15-20 prospects to reviewing AI insights for 60-80 prospects in 30 minutes. That frees up tons of time for actual selling.

**Look Like a Pro:** I'll walk into every conversation as someone who's done their homework. I'll build trust faster and spend my energy on building relationships instead of digging through company websites.

**Consistent Results:** My performance becomes predictable regardless of whether I'm having a good day or not. I get measurable improvement in my numbers and show I know how to use technology to get results.

### 📸 **Screenshots**

![alt text](image-2.png)