# Event Support Desk – Library Index

This Prompt Library contains five reusable templates for handling event attendee questions, improving message tone, protecting personal details, translating approved announcements, and preparing an event Q&A guide.

## Templates

| Template | Task | Variables | Version | Status |
|---|---|---|---|---|
| [EV-Reply-attendees](templates/EV-Reply-attendees-v1_2026_10_15.md) | Reply to attendee inquiries using approved Event Facts and one next step | `[INPUT_TEXT]` `[LANGUAGE]` `[TONE]` `[MAX_WORDS]` `[FACTS]` | v1 | Tested |
| [EV-Calm-Masseage](templates/EV-Calm-Masseage-v1_2026_10_15.md) | Rewrite staff messages into calm, polite replies | `[INPUT_TEXT]` `[LANGUAGE]` `[TONE]` `[MAX_WORDS]` `[FACTS]` | v1 | Tested |
| [EV-Mask-Details](templates/EV-Mask-Details-v1_2026_10_15.md) | Replace attendee names, emails, and phone numbers with safe codes | `[INPUT_TEXT]` `[LANGUAGE]` `[TONE]` `[MAX_WORDS]` `[FACTS]` | v1 | Tested |
| [EV-Bilingual-Announcement](templates/EV-Bilingual-Announcement-v1_2026_10_15.md) | Translate approved event announcements between Arabic and English | `[INPUT_TEXT]` `[LANGUAGE]` `[TONE]` `[MAX_WORDS]` `[FACTS]` `[APPROVAL_STATUS]` | v1 | Tested; review approval handling |
| [EV-Guide-Q&A](templates/EV-Guide-Q&A-v1_2026_10_15.md) | Turn five common attendee questions into a short Q&A guide | `[INPUT_TEXT]` `[LANGUAGE]` `[TONE]` `[MAX_WORDS]` `[FACTS]` | v1 | Tested; review bilingual word count |

*Links above are intended folder paths. Ensure the template files use these names before distributing the index.*

## Shared blocks

| Block | Used by | File |
|---|---|---|
| Approved Event Facts (v1) | All five templates | `blocks/Event-Facts-v1_2026_10_15.md` |

### Approved Event Facts

- The support desk opens at 07:30 on event day and stays open until the last session ends.
- Badges are collected at the entrance using the registration email.
- A ticket can be transferred to another person at least 48 hours before the event.
- The session schedule is published in the event app and can change.
- The desk cannot see the status of refunds. Refer the attendee to the finance team.
- Questions before the event are answered within 1 working day.
- The desk never asks for ID numbers, passwords or bank details.

## Rules

| File | What it is |
|---|---|
| `rules/Event-Desk-Rules-v1_2026_10_15.md` | Responsible-use rules: use approved facts, avoid promises, protect personal data, refer missing information to official channels, and review outputs |

## How to use

1. Select the template that matches the attendee-support task.
2. Copy the template into ChatGPT and fill in its input variables.
3. Choose the language, tone, and maximum word count.
4. Use the approved Event Facts; do not invent missing information.
5. Check the response for accuracy, privacy, and format before sharing it.

## `[LANGUAGE]` values (same in every template)

| Value | Meaning |
|---|---|
| Arabic | Answer in Arabic only |
| English | Answer in English only |
| Automated | Reply in the main language of the input |
| Bilingual | Two separate versions: Arabic and English |
| Mixed | One response combining Arabic and English |

## Test results

| Template | Prompt quality | Template quality | Output quality |
|---|---|---|---|
| EV-Reply-attendees | 5/5 | 6/6 | 5/5 |
| EV-Calm-Masseage | 5/5 | 6/6 | 5/5 |
| EV-Mask-Details | 5/5 | 6/6 | 5/5 |
| EV-Bilingual-Announcement | 5/5 | 6/6 | 5/5 |
| EV-Guide-Q&A | 5/5 | 6/6 | 5/5 |

*Scores are transcribed from the Test Results Report. Review noted issues before final approval.*

## Archive

Keep older template and Event Facts versions in `templates/_archive/` and `blocks/_archive/` when updates are made. No earlier versions are listed in this index.

## Change log

| Date | Change |
|---|---|
| 2026_10_15 | Created Event Support Desk library index with five event-specific templates |
| 2026_10_15 | Added shared Event Facts, language options, usage steps, and test-result summary |

**Owner:** Khawla Alomari · **Version:** v1 · **Date:** 2026_10_15
