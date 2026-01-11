# Email-Phishing-Detection-Lab

## Overview
In this lab, I analyzed a series of emails received by an executive inbox to identify social engineering attacks, phishing attempts, malware delivery methods, and legitimate internal communications. Acting as an IT security administrator, the objective was to determine whether each email posed a security risk and to take appropriate action by either deleting or keeping the message.

This lab focused on **behavioral analysis and decision-making**, not automated filtering, mirroring how real-world security teams evaluate email threats.

---

## Scenario
A company executive reported receiving multiple suspicious emails. As the IT security administrator, I was responsible for reviewing each message to determine whether it was legitimate or a social engineering attempt, and then handling it accordingly.

The evaluation was based on observable indicators such as sender identity, domain validity, language patterns, urgency, attachments, and links.

---

## Methodology
Each email was analyzed using the following criteria:

- Sender name vs. sender email domain validation
- Presence of suspicious attachments (e.g., executable files)
- Embedded or disguised links
- Use of urgency, fear, authority, or incentives
- Targeting of executives or internal employees (spear phishing / whaling)
- Consistency between message content and sender role
- Identification of hoaxes and forward-based chain emails
- Avoidance of false positives by recognizing legitimate internal communications

Decisions were made using **risk-based reasoning**, similar to how a SOC analyst or security administrator would operate in a production environment.

---

## Email Analysis Summary

| Email Type | Screenshot Filename | Action Taken | Key Indicators |
|-----------|---------------------|-------------|----------------|
| Fake Software Update (Phishing) | `FirstDeleted.png` | Deleted | Impersonation of Microsoft, unsafe update delivery |
| Malware Attachment | `hamsterexe.png` | Deleted | `.exe` attachment sent via email |
| Whaling (Executive Targeting) | `whalingexample.png` | Deleted | Executive-focused lure, external email domain |
| HR Impersonation (Ethics Video) | `legithr.png` | Kept* | Legitimate HR context, no credential request |
| Financial Phishing | `creditunionscam.png` | Deleted | Credential harvesting, urgency, fake authority |
| Virus Hoax / Chain Email | `grandma.png` | Deleted | Fear-based messaging, request to forward |
| Forward-Based Scam | `forwardscam.png` | Deleted | Incentive-based forwarding as payload |
| Curiosity-Based Malware Lure | `saragoodwin.png` | Deleted | Vague language, suspicious attachment |
| Legitimate Internal Announcement | `pumpkin.png` | Kept | No links, no attachments, benign request |
| Legitimate Internal Communication | `bob.png` | Kept | Normal workplace message, no exploit vector |

\* *Note: Link verification via hover inspection was unavailable in the lab environment. In a real-world setting, this email would warrant secondary verification rather than blind trust.*

---

## Tools & Skills Demonstrated
- Phishing and social engineering detection
- Spear phishing and whaling identification
- Email attachment and link risk analysis
- Domain and sender validation
- Hoax and misinformation recognition
- False positive avoidance
- Risk-based security decision-making

---

## Why This Is Important
Social engineering remains one of the most effective attack vectors used in real-world breaches. Organizations rely on security professionals to accurately identify malicious emails while avoiding unnecessary disruption caused by false positives.

This lab demonstrates the ability to:
- Think critically under uncertainty
- Distinguish legitimate business communications from threats
- Protect users and systems from credential theft, malware infection, and misinformation
- Apply security judgment beyond automated filtering tools

These skills are essential for entry-level security, SOC, and IT security roles.

---

## Disclaimer
All emails analyzed in this lab were part of a controlled training environment. No real systems or users were involved.
