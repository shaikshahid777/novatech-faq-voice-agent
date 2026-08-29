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
