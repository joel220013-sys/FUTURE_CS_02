# Phishing Email Detection & Awareness System

A phishing email analysis and awareness report prepared for Future Interns Cyber Security Task 2 (2026).

## Report

- [Phishing Email Awareness Report (PDF)](Phishing_Email_Awareness_Report.pdf)

## Scope and method

I reviewed public educational email samples and the synthetic account-lock example in the task. I inspected the visible sender details, message text, link text, and the authentication results included in one sample’s headers.

I did not open links or attachments. The sample uses placeholder domains and IP addresses, so its real-world sender or link reputation could not be verified.

## Tools

- Browser: reviewed public sample pages and email text
- Google Admin Toolbox Messageheader: tried with the sample headers; it could not recognize them, so no analyzer result is claimed

## Samples and sources

- Voice-message sample: [autinerd/phishing-mail-examples](https://github.com/autinerd/phishing-mail-examples/tree/main/voice-message)
- Fax-message sample: [autinerd/phishing-mail-examples](https://github.com/autinerd/phishing-mail-examples/tree/main/new-fax-message)
- Account-lock example: synthetic example supplied in the task; not a real collected email

The public repositories are cited as learning sources. Their raw email samples are not copied into this repository.

## Findings

The report explains the indicators, risk classifications, limitations, and practical prevention steps for each example. The voice-message sample’s displayed authentication results show SPF fail, no DKIM signature, and DMARC fail. The header analyzer did not independently verify those results.

## Safety

All links are shown as text for analysis. Do not visit suspicious links or open unexpected attachments.
