# Personal Task App

> A lightweight personal task manager: quick capture, open items and done items. Built to stay simple.
>
> **Type:** personal tool · **Stack:** Google Apps Script, Google Sheets, HTML Service · **My role:** idea and build

## The problem

A support supervisor collects dozens of small to-dos every day. Large project tools end up abandoned.

## The solution

- Started as an AI-built prototype and was moved to its own Apps Script web app, following the same architecture as the [investigation log](02-investigation-log.md).
- Each task stores priority, due date, note and source.
- **Postpone counter:** shows what I keep pushing back.
- Recurring tasks create their next occurrence automatically.
- Soft delete: nothing is lost.
- **A separate test spreadsheet**, so changes are checked without touching real data.

## Next step

Connect it to an AI assistant to ask "what is overdue today?" and create tasks by chat.
