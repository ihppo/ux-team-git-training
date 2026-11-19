---
name: harmonize-mockup-content
description: Harmonizes the fake content in mockups so names, people, dates, prices, copy and data stay consistent and realistic across every screen. Use when the user asks to harmonize, clean up, unify or make placeholder content consistent, or to remove lorem ipsum.
---

# Harmonize mockup content

Make all placeholder content in the selected frames (or the current page if nothing is selected) feel like it comes from **one coherent, believable product: Satisfactory**. Fix inconsistencies directly in the file, then report what changed.

Locale: **English (en-US)** for all content and formats.

## Workflow

1. **Inventory.** Read every text layer in scope, screen by screen. Note which component or instance each one belongs to.
2. **Build the content registry.** Before changing anything, decide the canonical values the whole file will share (see "Content registry" below). Reuse what already exists in the file: if "Sarah Chen" appears on 4 screens and "Jane Doe" on 1, Sarah Chen wins. Only invent new values when nothing usable exists.
3. **Detect issues.** Compare every text layer against the registry and the rules below.
4. **Fix directly.** Replace the text in the file. Respect the constraints in "Editing safely."
5. **Report.** End with a short summary (see "Final report").

## Content registry

Establish these once and reuse them everywhere:

- **Cast of personas.** A main user (the logged-in person) plus 5 to 10 secondary people. Each persona has a fixed full name, first name, initials, email, job title, company and avatar. The same person always has the same details on every screen.
- **The product.** One product name, one company name, one domain.
- **Reference date ("today").** One date the whole file treats as today. All relative dates ("2 hours ago", "Yesterday") and absolute dates must agree with it.
- **Key records.** Order numbers, invoice IDs, project names, account balances: anything that appears on more than one screen gets one canonical value.

## Rules

### People and personas
- Same person = same full name, spelling, initials, email, avatar and title everywhere.
- Initials in avatars match the name (Sarah Chen → SC).
- Use a varied, realistic cast (mixed origins and genders). No celebrities, no real public figures, no joke names ("John Doe", "Test User", "Foo Bar").
- Emails follow one pattern: `firstname.lastname@` or `firstname@`, on a reserved domain such as `example.com` or a fictional company domain.
- Avatars: one photo or one initials style per person; do not swap a person's photo between screens.

### Formats (en-US)
- Dates: `Oct 20, 2026` in UI, `10/20/2026` only in dense tables. Pick one style per context and stick to it.
- Time: 12-hour clock, `9:41 AM`.
- Currency: `$1,250.00`. Use cents only where the context needs them (invoices, payments); round elsewhere.
- Numbers: comma as thousands separator, period as decimal (`12,480.5`).
- Phone numbers: `(555) 010-0000` range (reserved for fiction).
- Addresses: realistic US format, fictional street numbers: `1240 Maple Ave, Portland, OR 97205`.
- Units: imperial unless the product clearly uses metric; never mix.

### Copy and tone
- Replace every lorem ipsum, "Text", "Title", "Label", "Lorem", "XXX" or "Placeholder" with realistic content that fits the screen's purpose.
- Content length should be realistic: a product title is not 2 words on one screen and 40 on another unless that is intentional to test overflow.
- Keep one voice across the file (same level of formality, same capitalization style). Use sentence case for UI labels and buttons unless the file clearly uses title case.
- The same action uses the same word everywhere (don't mix "Delete" and "Remove" for the same action).

### Data coherence
- Totals add up: line items sum to the subtotal; subtotal + tax + shipping = total.
- Counts match: a badge saying "3" means 3 items in the list it refers to.
- The same record shows the same values on list, detail and confirmation screens.
- Timelines are chronological and consistent with the reference date. Nothing happens in the future unless it is scheduled.
- Statuses make sense (an order can't be both "Delivered" and "Shipping soon").
- Charts and the numbers next to them agree.

## Editing safely

- Change **text content only**. Do not alter fonts, sizes, colors, styles, auto layout or component structure.
- If a text layer belongs to a **main component**, edit the instances, not the main component, unless the placeholder is in the main component itself and is clearly fake.
- Keep text roughly the same length as the original to avoid breaking layouts. If a fix would overflow its container, choose a shorter equivalent.
- Leave alone: intentional edge cases (very long names used to test truncation, empty states, error messages), buttons and navigation labels, and any layer whose name or nearby annotation indicates it is final or approved copy.
- Leave real brand names and legal text untouched.

## Final report

After editing, give a short summary:

1. The registry you used (cast of personas, product name, reference date, key records).
2. The number of text layers changed, grouped by category (people, formats, copy, data).
3. Anything you did **not** fix and why (e.g., possible intentional edge case, text locked, ambiguity between two equally used values).
