# AI LinkedIn Post Generator - Workflow Overview

## Project Overview

The **AI LinkedIn Post Generator** is an automated content creation workflow built using **n8n** and **Google Gemini AI**. The workflow transforms a user-provided topic into a professional, engaging, and LinkedIn-ready post using multiple specialized AI agents.

The system follows a modular AI agent architecture, where each agent is responsible for a specific task in the content generation pipeline.

---

# Workflow Architecture

```
                    +----------------+
                    |  User Input    |
                    | (Topic/Prompt) |
                    +-------+--------+
                            |
                            ▼
                 +----------------------+
                 | Research AI Agent    |
                 +----------+-----------+
                            |
                            ▼
                 +----------------------+
                 | Summary AI Agent     |
                 +----------+-----------+
                            |
                            ▼
                 +----------------------+
                 | LinkedIn Writer      |
                 +----------+-----------+
                            |
                            ▼
                 +----------------------+
                 | Hashtag Generator    |
                 +----------+-----------+
                            |
                            ▼
                 +----------------------+
                 | Image Prompt Agent   |
                 +----------+-----------+
                            |
                            ▼
                 +----------------------+
                 | Final Output         |
                 +----------------------+
```

---

# Workflow Steps

## Step 1 — User Input

The workflow begins when a user submits a topic or idea for a LinkedIn post.

**Example Input**

```
Artificial Intelligence in Healthcare
```

---

## Step 2 — Research Agent

The Research Agent gathers relevant information about the topic.

It focuses on:

- Latest industry trends
- Important statistics
- Market insights
- Benefits
- Challenges
- Real-world applications

The goal is to collect factual and reliable information before content generation.

---

## Step 3 — Summary Agent

The Summary Agent analyzes the research and extracts the most valuable insights.

It organizes the information into a structured summary that is easier for the content generation agent to understand.

---

## Step 4 — LinkedIn Content Generator

Using the summarized research, the AI generates a professional LinkedIn post.

The generated post includes:

- Attention-grabbing hook
- Valuable insights
- Professional tone
- Clear formatting
- Call-to-action (CTA)

---

## Step 5 — Hashtag Generator

The workflow generates relevant hashtags based on the post topic.

The hashtags improve discoverability and engagement on LinkedIn.

Example:

```
#ArtificialIntelligence
#MachineLearning
#Innovation
#DataScience
#Technology
```

---

## Step 6 — Image Prompt Generator

The workflow creates a detailed AI image prompt that can be used with image generation models such as DALL·E, Midjourney, or Flux.

The generated prompt matches the LinkedIn post content.

---

## Step 7 — Final Output

The workflow produces:

- LinkedIn Post
- Suggested Hashtags
- AI Image Prompt

These outputs can be published directly or reviewed before posting.

---

# Technologies Used

- n8n
- Google Gemini API
- HTTP Request Nodes
- AI Agent Workflows
- Prompt Engineering
- JSON
- Markdown

---

# Workflow Features

- Automated AI research
- Multi-agent architecture
- Professional LinkedIn post generation
- Intelligent summarization
- Automatic hashtag generation
- AI image prompt creation
- Modular prompt design
- Easy customization
- Reusable workflow
- Scalable architecture

---

# Use Cases

This workflow can be used by:

- Content Creators
- Marketing Professionals
- Entrepreneurs
- Personal Branding Experts
- Students
- Freelancers
- Recruiters
- AI Enthusiasts

---

# Future Enhancements

Planned improvements include:

- Multi-language support
- Support for X (Twitter), Instagram, and Facebook
- AI-generated images
- Post scheduling
- SEO optimization
- Analytics dashboard
- Multiple writing styles
- Brand voice customization
- Web search integration
- Content calendar automation

---

# Repository Structure

# Notes

- This project is designed for educational and portfolio purposes.
- API credentials are not included in the repository.
- Users must configure their own API keys before running the workflow.
- The workflow is fully customizable and can be extended with additional AI agents.
