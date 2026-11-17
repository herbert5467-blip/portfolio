# Field Service Evidence Audit

> Automatic comparison between what each work order checklist requires and what the technician actually sent, to find services closed without proof.
>
> **Type:** data analysis · **Stack:** BigQuery (SQL), Google Sheets · **My role:** defined the criteria and the validation process

## The problem

Warranty and field-visit work orders have an evidence checklist, such as "video of the machine working after the part was replaced". In practice, photos arrived where a video was required, or nothing arrived, and the work order was closed anyway.

## The solution

1. A BigQuery query over work orders and their checklists.
2. For each field, compare the **file type required** with the **file type received**.
3. Group cases by type of gap, for example "no proof the machine works".
4. Check whether the same machine had **a new ticket within a short window**, a sign the service may not have fixed the problem.
5. Produce a validation sheet where the supervisor marks Yes, No or Unsure and adds a note.

The criterion is stated in the sheet itself: the check compares file types and does not open the photo or video.

## What I learned

- An audit is more useful when the person who acts on it can see the rule behind every flag.
- Linking "evidence missing" to "the customer called again" turns a compliance check into a quality signal.
