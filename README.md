# hotel-info-agent
An AI-powered virtual assistant designed to support hotel guests by providing clear, accurate, and welcoming responses to common questions about hotel services, policies, and amenities.

## Overview
The Hotel Information Agent acts as a digital front desk, helping guests quickly find information without waiting for staff assistance. The agent is designed with a hospitality-focused personality and emphasizes accuracy, safety boundaries, and a positive guest experience.

## Features
- Answers guest questions about hotel amenities (e.g., pool, spa, WiFi)
- Provides restaurant hours and dining information
- Responds to check-in and check-out policy inquiries
- Supports multilingual guest interactions
= Uses grounded responses based on verified hotel knowledge

## Architecture and Technologies
- Platform: Azure AI Foundry
- Model: GPT-5-mini
- Agent Instructions:  You are a polite, professional, and welcoming assistant for a hotel. Your goal is to provide helpful, accurate information about the hotel’s amenities, policies, and local attractions while respecting safety and privacy boundaries.
- Core Capabilities:
  - Prompt-based agent configuration
  - Knowledge grounding via uploaded hotel documents
  - Language detection and translation
  - Evaluation and testing via Playground and Evaluation tools

## Demonstration
- Placeholder for video

## Lessons Learned
1. Agent Boundaries Are Critical
Clear boundaries prevent the agent from giving unsafe or inappropriate responses (for example, medical or legal advice). Explicit escalation and fallback instructions are essential for maintaining trust.

2. Prompt Engineering Drives Reliability
Well-structured prompts significantly reduce hallucinations and improve tone consistency. Small prompt changes can have large impacts on accuracy and user experience.

3. Multilingual Support Requires Workflow Design
Supporting languages beyond English is more than translation. Language detection, translation, entity extraction, and replying in the guest’s language must work together to ensure clarity.

4. The Playground Enables Rapid Iteration
Using the Playground allowed fast experimentation with tone, response length, and edge cases before committing to persistent agent configurations, reducing deployment risk.

5. Testing Beyond the Happy Path Matters
Testing only standard questions is insufficient. Including edge cases (ambiguous requests, emergencies, unclear inputs) ensures the agent behaves safely and consistently in real-world use.

6. Knowledge Quality Directly Impacts Answer Quality
Accurate, well-organized, and up-to-date documents are essential. After every update, testing with targeted queries confirms the agent is grounded in the correct information.

## Future Enhancements
- Integration with booking and reservation systems
- Expanded personalization based on guest preferences
- Analytics on common guest questions to improve hotel operations
