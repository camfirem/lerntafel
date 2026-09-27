<!-- DRAFT: not legal advice. Have this reviewed before the first public release, in particular the "no telemetry" claim and the GDPR data-controller wording. -->

# Privacy Notice

This notice explains what happens to your data when you use Lerntafel. It applies to the beta described in [README.md](README.md) and is governed by the same license terms ([LICENSE.md](LICENSE.md)).

## Who is responsible

Mark Friedrichs is the sole developer and responsible party (data controller under GDPR, Art. 4 No. 7) for the Lerntafel software itself. Contact: see [Feedback](README.md#feedback) / [GitHub Issues](../../issues). <!-- TODO: add a postal address here if this ever becomes legally required -->

## What Lerntafel stores locally

- Boards, drawings, imported PDFs, settings and chat history are saved as files **on your own computer**, in a folder you choose or the application default.
- API keys you enter (Anthropic, OpenAI, or other providers) are stored **locally on your computer only**. They are never sent to the developer.
- Lerntafel does not create a user account and does not require you to sign in to use the whiteboard, PDF or drawing features.

## What leaves your computer

- **Without the AI chat, or with a local Ollama model:** nothing leaves your computer. Lerntafel makes no network calls of its own for its core features.
- **With the AI chat and a cloud provider (Anthropic or OpenAI, using your own API key):** the visible part of your board, your typed message and the recent chat context are sent to that provider's servers to generate a response. That provider then processes this data under **its own** privacy policy and terms, not Lerntafel's:
  - Anthropic: <https://www.anthropic.com/legal/privacy>
  - OpenAI: <https://openai.com/policies/privacy-policy>
- If you use the optional document-library feature, the documents you import may also be included in what is sent to the provider when the chat cites them.
- Lerntafel itself does not log, collect or forward this traffic anywhere else; it is a direct connection between your computer and the provider you configured, using your own API key/account.

## Telemetry and analytics

Lerntafel does not collect usage statistics, crash reports or analytics, and does not phone home to the developer. <!-- TODO: confirm this is still true right before release; update here immediately if that changes in any version -->

## Children's privacy

Lerntafel is a general-purpose whiteboard tool. It is not directed at children and collects no personal data of its own; any data sent to an AI provider under "What leaves your computer" is subject to that provider's own terms, which may set a minimum age.

## Changes to this notice

If a future version changes what data is stored or transmitted, this file will be updated and the change noted in [CHANGELOG.md](CHANGELOG.md).
