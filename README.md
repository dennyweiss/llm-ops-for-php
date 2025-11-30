# LLM Ops for PHP

A debugging and evaluation platform for AI-powered services, built on Laravel. Designed for civic tech organizations that need GDPR-compliant AI integration with verifiable response quality.

## The Problem

Civic organizations helping citizens navigate bureaucracy face two barriers to AI adoption:

1. **Data Protection**: Citizen conversations contain sensitive personal information. Sending this data to external AI providers violates GDPR requirements.
2. **Reliability**: Without tools to test and debug AI responses, domain experts cannot verify quality. Wrong answers about benefit deadlines or legal rights cause real harm.

Existing evaluation platforms (Langfuse, LangSmith, Opik) require Python infrastructure—impractical for organizations running TYPO3 or Drupal.

## What We're Building

A PHP-native platform that sits between chat interfaces and AI providers:

- **PII Pseudonymization**: Microsoft Presidio removes personal data before LLM processing; reconstructs it in responses
- **Conversation Tracing**: Capture every exchange for analysis and debugging
- **Evaluation Interface**: Domain experts rate responses via FilamentPHP admin—no coding required
- **Prompt Testing**: Replay conversations against prompt variations to identify failure patterns
- **Multi-Provider Support**: Connect to OpenAI, Anthropic, Mistral, or local models via Neuron AI/Prism PHP

Distributed as a Composer package with an embeddable chat widget for TYPO3/Drupal sites.

## Status

🚧 **Pre-development** — Application submitted to [Prototype Fund](https://prototypefund.de/) (Class 02).

## Team

- **Denny Weiß** - [LinkedIn](https://www.linkedin.com/in/denny-weiss/)
- **Martin Sigloch** - [LinkedIn](https://www.linkedin.com/in/martin-sigloch/)
- **Franziska Liebenow-Rudolph** - [LinkedIn](https://www.linkedin.com/in/franziska-liebenow-rudolph/)

## License

MIT License
