# Changelog

## v1.0 - first public release

- Search the raw MailEnable SMTP, POP and IMAP Activity logs (and optionally Debug logs) for any text, over the recent days, every available day, or one day picked from the log days that exist on the server. Optional regex.
- **Result** column: EHLO refused, Login failed (535), Rejected (550), Temp refused (4xx).
- **Only EHLO refused**: lists the connections MailEnable refused at EHLO/HELO, with the EHLO name and the entry of your *EHLO strings to block* list that caught it (read from the registry, read only). **Summary** groups the refused names and the busiest IPs.
- **From**, **To** and **Find** boxes: message-level search, one row per message, every box you fill must match.
- **Trace mail**: one combined, copyable report per mail - SMTP transaction, MTA / filter / debug log lines for the same Message ID and the outbound copies MailEnable made of it - with a RESULT line (refused, accepted, deleted by a filter, relayed, not received...).
- Date and time columns, click-to-sort headers, CSV / text export, About box.
- The Trace mail button is disabled and a message is shown while a trace runs.
