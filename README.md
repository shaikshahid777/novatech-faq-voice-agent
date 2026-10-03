<!-- SHOWCASE_START --><div align="center">[![Typing](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=22&duration=2800&pause=900&color=58A6FF&center=true&vCenter=true&width=900&lines=novatech%20faq%20voice%20agent;AI%20%7C%20Automation%20%7C%20Engineering;Explore%20the%20project%20%F0%9F%9A%80)](https://github.com/shaikshahid777/novatech-faq-voice-agent)<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:161B22,100:58A6FF&height=110&section=header&text=novatech-faq-voice-agent&fontSize=26&fontColor=FFFFFF&animation=twinkling&fontAlignY=65" width="100%" alt="Animated project banner"/>

[![Repository](https://img.shields.io/badge/Repository-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/shaikshahid777/novatech-faq-voice-agent) [![Issues](https://img.shields.io/badge/Report-Issue-red?style=for-the-badge&logo=github)](https://github.com/shaikshahid777/novatech-faq-voice-agent/issues/new) [![Stars](https://img.shields.io/github/stars/shaikshahid777/novatech-faq-voice-agent?style=for-the-badge&logo=github)](https://github.com/shaikshahid777/novatech-faq-voice-agent/stargazers) [![Fork](https://img.shields.io/github/forks/shaikshahid777/novatech-faq-voice-agent?style=for-the-badge&logo=github)](https://github.com/shaikshahid777/novatech-faq-voice-agent/fork) [![Profile](https://img.shields.io/badge/Profile-Visit-0A66C2?style=for-the-badge&logo=github)](https://github.com/shaikshahid777)</div>

> ✨ **Project Showcase Mode:** animated banner • interactive navigation • live repository actions

[🚀 Repository](https://github.com/shaikshahid777/novatech-faq-voice-agent) · [🐞 Report Issue](https://github.com/shaikshahid777/novatech-faq-voice-agent/issues/new) · [⭐ Star](https://github.com/shaikshahid777/novatech-faq-voice-agent/stargazers) · [🔱 Fork](https://github.com/shaikshahid777/novatech-faq-voice-agent/fork) · [👤 Profile](https://github.com/shaikshahid777)

<!-- SHOWCASE_END -->

# NovaTech FAQ Welcome Agent

## Inbound Voice Agent Capstone

A production-style inbound AI voice assistant built in Vapi for NovaTech Solutions. The assistant is designed to provide a professional welcome, answer predefined FAQs, handle unclear questions, provide safe fallback responses, support escalation requests, and close calls professionally.

## Demo

Loom demo: https://www.loom.com/share/361790c8bc3c472d91b47cc479d268be

## Assistant Configuration

- Assistant: FAQ Welcome Agent
- LLM: GPT-4.1
- Transcriber: Deepgram Nova-2
- Language: English
- Voice: ElevenLabs Multilingual v2 / Bella
- Maximum duration: 300 seconds
- Silence timeout: 30 seconds

## Intent Handling

### FAQ MATCH
Answers only from the predefined FAQ knowledge base.

### UNCLEAR
Politely asks the caller to clarify when the request cannot be confidently understood.

### ESCALATION
Acknowledges requests for a human representative and directs the caller to customer support.

## FAQ Knowledge Base

| Question | Answer |
|---|---|
| What are your opening hours? | We are open Monday through Friday from 9 AM to 6 PM EST. |
| Where are you located? | Our main office is located at 100 Innovation Way, Suite 400, Austin, TX. |
| How can I contact customer support? | You can contact our customer support team through the support contact provided by NovaTech Solutions. |
| What services do you provide? | NovaTech Solutions provides technology and business solutions for its customers. |

## Fallback

The assistant is instructed not to fabricate information. For unsupported questions it uses:

> I'm sorry. I don't have that information available. Please contact our customer support team for further assistance.

## End Call Configuration

End-call phrases include:

- goodbye
- that's all I needed
- thank you goodbye
- bye
- have a good day

Closing message:

> Thank you for calling NovaTech Solutions. Have a wonderful day! Goodbye.

## Test Evidence

A simulated test demonstrated:

1. FAQ match — opening hours
2. FAQ match — location
3. FAQ match — customer support
4. FAQ match — services
5. Unclear request handling
6. Out-of-scope fallback handling
7. Escalation request handling
8. Professional call closure and call termination

## Phone Number

A Vapi free US phone number is configured and assigned to the FAQ Welcome Agent for inbound calling:

`+1 (810) 267-8220`

## Limitation

The Vapi free US number does not support outbound international calls to an Indian +91 number. Therefore, the demonstrated end-to-end validation uses the Vapi simulated/browser test environment rather than an international outbound PSTN test call.

## Submission Evidence

Configuration screenshots should cover:

- System prompt and FAQ knowledge base
- Model, transcriber, and voice settings
- First message and end-call settings
- Phone number and inbound assistant assignment
- Test conversation/transcript

## Security

Do not commit Vapi API keys, Twilio Auth Tokens, Telnyx API keys, passwords, or other credentials to this repository.
