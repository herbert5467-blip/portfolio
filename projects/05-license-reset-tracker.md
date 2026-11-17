# Supplier License Reset Tracker

> A small app to request and follow software license resets with a supplier, measuring internal time and supplier time separately.
>
> **Type:** internal tool · **Stack:** Google Apps Script, Google Sheets · **My role:** idea and build

## The problem

The [queue audit](04-support-queue-audit.md) showed that cases depending on a supplier license reset had one of the longest cycles and a high rate of customers coming back. Requests were tracked in a manual spreadsheet, so nobody could tell how much of the wait was ours and how much was the supplier's.

## The solution

- Every request gets an ID and stores requester, contract, software version, reason, attachment and status.
- The app calculates **hours in the internal queue**, **hours with the supplier** and **total hours**.
- Repeated requests for the same license are visible.
- The final result is recorded in plain text.

## Why it matters

Splitting internal time from supplier time changes the conversation: what is ours, we fix; what is the supplier's becomes a request backed by data.
