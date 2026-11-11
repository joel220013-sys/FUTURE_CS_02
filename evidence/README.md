# Task 2 Evidence Index

These files document the analyst's read-only review. They are not live mailbox captures. The public sample uses reserved `.example` domains and the documentation-range IP address `192.0.2.1`; treat them as educational placeholders, not active threat indicators.

## 1. Voice-message sample

- **Evidence image:** [voice-message-authentication-header.png](voice-message-authentication-header.png)
- **Source:** [message.eml in the public educational repository](https://github.com/autinerd/phishing-mail-examples/blob/main/voice-message/example1/message.eml)
- **What it supports:** the sample's displayed `Authentication-Results` line says SPF fail, DKIM none, and DMARC fail. The visible `From` and `Return-Path` use `target.example.com` placeholders.
- **Limit:** these values are read from the sample text; the email-header analyzer did not parse the submitted text and did not independently verify them.

## 2. Header analyzer attempt

- **Evidence image:** [google-header-analyzer-attempt.png](google-header-analyzer-attempt.png)
- **Tool:** Google Admin Toolbox Messageheader.
- **Observed result:** the page said it could not recognize the submitted email headers. No analyzer verdict is claimed.

## 3. Fax-message sample

- **Source:** [new-fax-message sample directory](https://github.com/autinerd/phishing-mail-examples/tree/main/new-fax-message)
- **What was recorded:** the report notes the unexpected fax notification, undisclosed recipients, a claimed PDF, and a placeholder destination. The link was not opened and the attachment was not downloaded.
- **Limit:** the source email is linked for attribution; its raw message is not copied into this repository.

## 4. Account-lock example

This is a synthetic example supplied in the Future Interns task prompt, not a real collected email. The report defangs its URL and classifies it as suspicious / likely phishing based on the example's wording and link text.
