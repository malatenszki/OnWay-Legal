# OnWay — Data Deletion Request

**App:** OnWay (driver safety alerts for Serbia and Hungary)
**Developer:** Malatenski David (Serbia, individual developer)
**Contact:** onway.help@proton.me

---

## How to delete your OnWay data

OnWay offers two ways to request deletion of your personal data. You may use either.

### Option 1 — In-app (preferred, immediate)

1. Open the OnWay app
2. Tap the settings icon (⚙) in the top-right of the map
3. Scroll down to the **Privacy** section
4. Tap **Delete my data**
5. Confirm on the dialog

Your data is deleted **immediately** (within a few seconds) when you tap confirm. No human review is required. The app regenerates a fresh anonymous device identity, so you can continue using OnWay afterwards if you wish — the new identity is unlinked from your previous one.

### Option 2 — Email request

If you have uninstalled the app and cannot access the in-app flow, send an email to:

> **onway.help@proton.me**

with the subject line **"OnWay — Delete my data"**. Please include:

- The approximate dates you used the app (to help locate your records)
- Any optional nickname you set in the app

We will process the request within **30 days** and reply with a confirmation when the deletion is complete, in accordance with GDPR Article 17 (Right to Erasure) and the Serbian Law on Personal Data Protection.

---

## What is deleted

The following personal data is **fully and permanently deleted**:

- Your anonymous device identity (UUID) and its associated Supabase auth record
- All hazard / accident / traffic / pothole / camera reports you submitted, including their location, timestamp, type and any optional text note
- All camera location suggestions you submitted
- Your optional nickname (if you set one)

## What is retained (anonymized)

For the integrity of the community-driven map, a small subset of your contributions is **kept in an anonymized form** — the personal identifier link is removed, but the data point itself remains and contributes to the shared map:

- **Confirmation votes** you cast on reports or cameras (confirm / deny). The aggregate count stays so other drivers still see which reports are community-verified, but the link to your device is removed.
- **Camera verification records** (for cameras that crossed the "verified" threshold because of your confirmations). Same treatment — the map-level verification state is preserved, personal link is removed.
- **Abuse reports** you submitted through the in-app "Report inappropriate" function, retained for moderation history. Your device identifier is removed from these records.

After anonymization these records cannot be used to identify you. Per GDPR Recital 26, anonymized data is no longer personal data.

## Retention period

Personal data (the "deleted" list above) is **deleted immediately** on request — there is no hold period.

Anonymized aggregate data (the "retained" list above) has no fixed retention period and is kept for as long as the OnWay service operates.

---

**Last updated:** 2026-04-14
