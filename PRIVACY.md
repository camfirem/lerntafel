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

- **Without the AI chat, or with a local Ollama model:** your boards, documents and messages never leave your computer. The only network call Lerntafel makes on its own is the update check described below.
- **Update check (since 0.9.6):** at most once a day when the app starts, and whenever you choose *Help → Check for updates*, Lerntafel downloads the public list of releases of this repository from GitHub (`api.github.com`). The request contains no board content, no settings and no personal data, only the usual technical data of a web request (your IP address and the app name and version, e.g. `Lerntafel/0.9.6`). GitHub processes it under its own privacy statement: <https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement>. The developer does not receive or log these requests.
- **With the AI chat and a cloud provider (Anthropic or OpenAI, using your own API key):** the visible part of your board, your typed message and the recent chat context are sent to that provider's servers to generate a response. That provider then processes this data under **its own** privacy policy and terms, not Lerntafel's:
  - Anthropic: <https://www.anthropic.com/legal/privacy>
  - OpenAI: <https://openai.com/policies/privacy-policy>
- If you use the optional document-library feature, the documents you import may also be included in what is sent to the provider when the chat cites them.
- Lerntafel itself does not log, collect or forward this traffic anywhere else; it is a direct connection between your computer and the provider you configured, using your own API key/account.

## Telemetry and analytics

Lerntafel does not collect usage statistics, crash reports or analytics, and does not phone home to the developer. The update check (see above) only reads GitHub's public release list; it reports nothing back. <!-- Checked for 0.9.6 (update check added). Update here immediately if that changes in any version. -->

## Children's privacy

Lerntafel is a general-purpose whiteboard tool. It is not directed at children and collects no personal data of its own; any data sent to an AI provider under "What leaves your computer" is subject to that provider's own terms, which may set a minimum age.

## Changes to this notice

If a future version changes what data is stored or transmitted, this file will be updated and the change noted in [CHANGELOG.md](CHANGELOG.md).
