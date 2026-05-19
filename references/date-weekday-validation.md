# Date And Weekday Validation

Use this whenever the answer includes dates, weekdays, business days, market days, publication dates, event dates, deadlines, or relative dates such as today, yesterday, tomorrow, this week, next month, or last quarter.

## Non-Negotiable Rule

Do not guess weekdays. Verify them.

If a source says both a date and a weekday, independently verify the weekday from the date. If they conflict, flag the mismatch instead of silently copying either value.

## Date Normalization

For every important date:

- Normalize to ISO format: `YYYY-MM-DD`.
- Include the weekday when relevant.
- Include timezone or geography when the date could differ by region.
- Keep publication date, event date, filing date, access date, and effective date separate.
- For relative dates, resolve them against the current date and timezone, then state the assumption.

## Weekday And Business-Day Checks

Separate:

- `weekday`: Monday through Friday by calendar.
- `business day`: a working day under a specific country, exchange, bank, or organization calendar.
- `market day`: an exchange trading day under a specific market calendar.

Do not call a date a business day or market day unless the relevant calendar/holiday status is checked or the source explicitly says so.

## Common Failure Modes

- Copying a source's weekday typo without verification.
- Mixing US/Japan/China timezones for events around midnight.
- Treating a weekday as a market day during holidays.
- Confusing announcement date, filing date, effective date, and article publication date.
- Using "today" from the source instead of the user's current date.

## Output Rules

When dates matter, include one of:

- `Date check: YYYY-MM-DD (Weekday, timezone/geography if relevant)`
- `Business-day status: checked against <calendar/source>`
- `Weekday mismatch: source says <weekday>, calendar check gives <weekday>`
- `Date location unavailable: source did not provide page/section/date metadata`

If you cannot verify the weekday, do not state it confidently. Mark it as `not verified`.
