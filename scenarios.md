# Scenario Bank — Threat Hunt Ready

Fictional examples for defensive training. Follow approved local procedures.

## 1. Urgent account warning

**Category:** Email security · **Level:** Awareness

**Scenario:** An email says your company account will be disabled in 30 minutes and links to an unfamiliar sign-in page. The sender address is subtly different from the real one.

**Question:** What is the safest next step?

- A. Click the link and sign in before the deadline.
- B. Reply to the sender to ask if it is genuine.
- C. Avoid the link and report the message through the approved channel.
- D. Forward the message to the whole department.

**Best answer:** C

**Explanation:** Urgency, an unfamiliar URL, and a subtly different sender address are phishing indicators. Report it through the approved process and do not interact with links or attachments.

**Key takeaway:** Verify through a known official route and report suspicious messages rather than spreading them.

---

## 2. MFA prompts you did not request

**Category:** Identity security · **Level:** Awareness

**Scenario:** You receive several multi-factor authentication approval prompts even though you are not trying to sign in.

**Question:** What should you do?

- A. Approve one prompt to stop the notifications.
- B. Deny the prompts and promptly report them to IT/security.
- C. Post a screenshot publicly to ask what it means.
- D. Turn off MFA permanently.

**Best answer:** B

**Explanation:** Unexpected repeated MFA prompts may indicate a compromised password or an MFA-fatigue attempt. Deny them and report the event.

**Key takeaway:** Never approve a sign-in you did not initiate.

---

## 3. Files suddenly become unreadable

**Category:** Endpoint response · **Level:** Awareness

**Scenario:** A workstation starts renaming many files and a ransom note appears after an unexpected attachment was opened.

**Question:** What is the best response?

- A. Keep working and delete the note.
- B. Download a random cleanup tool and run it.
- C. Alert security immediately and follow incident-response instructions, including any policy-directed isolation.
- D. Copy affected files to personal cloud storage.

**Best answer:** C

**Explanation:** Mass file changes and a ransom note may indicate ransomware. Promptly contact responders and avoid improvised cleanup.

**Key takeaway:** Escalate suspected ransomware immediately; do not experiment with cleanup tools.

---

## 4. The found USB drive

**Category:** Removable media · **Level:** Awareness

**Scenario:** You find a USB drive labelled “Payroll—urgent” in a meeting room and have access to a work laptop.

**Question:** What is the safest action?

- A. Plug it in but do not open files.
- B. Use a personal computer to inspect it.
- C. Give it to the designated IT/security contact without connecting it to a device.
- D. Ask coworkers to try it.

**Best answer:** C

**Explanation:** Unknown removable media can contain malicious files or be part of social engineering. Do not connect it to a device.

**Key takeaway:** Never plug in found or untrusted USB devices.

---

## 5. A login at an unusual time

**Category:** Introductory threat hunting · **Level:** IT + Security

**Scenario:** An authorized analyst sees a successful login at 02:13 from an unfamiliar location. The employee usually works local business hours. This single indicator does not prove compromise.

**Question:** What is the most defensible next step?

- A. Conclude the account is compromised based only on location.
- B. Correlate approved identity, device, VPN, MFA, and related activity logs, then follow escalation procedures.
- C. Delete the event to reduce noise.
- D. Contact the employee using details from the suspicious event.

**Best answer:** B

**Explanation:** Threat hunting validates a lead using context and multiple sources. Check the timestamp, source, device, MFA and VPN context within authorized tools.

**Key takeaway:** An anomaly is a lead, not a verdict. Correlate telemetry before drawing conclusions.

---

## 6. Unexpected outbound data transfer

**Category:** Data protection · **Level:** IT + Security

**Scenario:** A monitoring dashboard shows a workstation transferring much more data to an unfamiliar external destination than usual. The owner does not recognize the upload.

**Question:** What should the analyst do next?

- A. Publicly accuse the employee.
- B. Record time, host, destination, volume and related alerts; validate business context and escalate under policy.
- C. Ignore it because HTTPS is encrypted.
- D. Copy the data to a personal account for inspection.

**Best answer:** B

**Explanation:** An unusual transfer may be benign or suspicious. Preserve relevant metadata, check approved business context, and follow authorized investigation procedures.

**Key takeaway:** Use minimum necessary evidence and protect sensitive data.

---

## 7. A request to install a helper tool

**Category:** Software security · **Level:** Awareness

**Scenario:** A caller claiming to be from IT asks you to install a remote-access tool from a file-sharing link. No normal IT ticket or announcement exists.

**Question:** What should you do?

- A. Install it because the caller knows the company name.
- B. Ask the caller to email the link, then install it.
- C. Verify the request through a known internal IT channel before installing anything.
- D. Test it on another company device.

**Best answer:** C

**Explanation:** Attackers may impersonate IT staff to gain remote access. Independently verify identity and authorization and install only approved software.

**Key takeaway:** Verify identity and authorization before granting access or installing software.

---

## 8. A suspicious process chain

**Category:** Endpoint telemetry · **Level:** IT + Security

**Scenario:** An endpoint alert shows an office application launching a command interpreter, which starts an unfamiliar script. The alert is not confirmed as malicious.

**Question:** What is the best introductory hunting approach?

- A. Treat it as confirmed malware and wipe the machine immediately.
- B. Review process ancestry, command-line details, file/signature information, user context and related alerts in authorized tools.
- C. Disable endpoint protection.
- D. Upload full endpoint logs to a public forum.

**Best answer:** B

**Explanation:** The process chain may be legitimate automation or abuse. Examine process lineage and correlated events, then document and escalate according to playbooks.

**Key takeaway:** Build a timeline from authorized telemetry; an alert is not proof by itself.

---

## 9. Access outside a person's role

**Category:** Insider-risk signals · **Level:** IT + Security

**Scenario:** A report shows an employee account reading many documents from a department the employee does not normally support. A temporary project may explain it.

**Question:** What is the most appropriate response?

- A. Accuse the employee of stealing data.
- B. Share the employee's name and file list in a public chat.
- C. Validate authorization and business context, preserve relevant audit evidence, and escalate through the defined process.
- D. Delete the account immediately without consulting responders.

**Best answer:** C

**Explanation:** Unusual access may be legitimate work, misconfiguration, compromise or misuse. Check approved context, protect privacy and escalate without assumptions.

**Key takeaway:** Investigate behavior, not assumptions about a person.

---

## 10. You clicked before you noticed

**Category:** Incident reporting · **Level:** Awareness

**Scenario:** You clicked a suspicious link and entered your work password. The page now looks fake, but nothing else seems to have happened.

**Question:** What should you do now?

- A. Wait a few days for signs of trouble.
- B. Delete the email and keep it private.
- C. Report it immediately and follow official instructions to secure the account.
- D. Send your password to IT so they can check it.

**Best answer:** C

**Explanation:** Report accidental clicks or credential disclosure promptly. Use official recovery instructions and never share your password.

**Key takeaway:** Fast, honest reporting matters more than blame.

---

