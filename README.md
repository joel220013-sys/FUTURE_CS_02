# Phishing Email Detection & Awareness System

A phishing email analysis and awareness report prepared for Future Interns Cyber Security Task 2 (2026).

## Report

- [Phishing Email Awareness Report (PDF)](Phishing_Email_Awareness_Report.pdf)

## Scope and method

I reviewed two public educational email samples and the synthetic account-lock example supplied in the task. I inspected the visible sender details, message text, displayed link text, and authentication results included in one sample's headers.

I did not open links or attachments. The sample uses placeholder domains and IP addresses, so real-world sender or link reputation could not be verified.

## Tools

- **Browser:** reviewed public sample pages and email text.
- **Google Admin Toolbox Messageheader:** attempted with the sample header text; it could not recognize the headers, so no analyzer verdict is claimed.

## Samples and sources

- **Voice-message sample:** [autinerd/phishing-mail-examples](https://github.com/autinerd/phishing-mail-examples/tree/main/voice-message).
- **Fax-message sample:** [autinerd/phishing-mail-examples](https://github.com/autinerd/phishing-mail-examples/tree/main/new-fax-message).
- **Account-lock example:** synthetic example supplied in the Future Interns task; not a real collected email.

The public repositories are cited as learning sources. Raw email files are not copied into this repository.

## Evidence

The [`evidence/`](evidence/) folder contains a cropped header excerpt from the voice-message educational sample, a screenshot of the header analyzer's parse failure, and an evidence index describing source and limitations. The fax-message analysis and the synthetic account-lock example are documented in the PDF; their source and status are recorded in `evidence/README.md`.

## Findings

The report explains phishing indicators, risk classifications, limitations, and practical prevention steps for each example. The voice-message sample's displayed authentication results show SPF fail, no DKIM signature, and DMARC fail. The header analyzer did not independently verify those values.

## Safety

Links are documented as text only. Do not visit suspicious links or open unexpected attachments.
