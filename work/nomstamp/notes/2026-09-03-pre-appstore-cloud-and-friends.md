# Notes

- **Goal:** NomStamp
- **Date:** 2026-09-03
- **Source:** product planning — core app done locally (map, stamp photo, view on map); app code lives in separate repo
- **Serves this goal by:** names what must ship before App Store so stamps are not lost and users can share — unblocks retention and word-of-mouth toward 100 returning users

## In my own words

NomStamp works locally: take a food photo, stamp it, see it on a map. Before App Store, it needs **identity**, **cloud backup**, and a **minimal sharing path**. Full social network is not required for v1.

Recommended stack for solo iOS: **Sign in with Apple + CloudKit** for backup/sync. Add a small backend (Firebase or Supabase) only when building the friend map — or use CKShare for lighter sharing first.

## Why it matters for the goal

Local-only storage blocks return use: users fear losing stamps on reinstall or new phone. No sharing blocks word-of-mouth. Both are retention/distribution problems, not polish.

## Pre-App Store tasks (in order)

### Phase 1 — Cloud backup (do first)

- [ ] Sign in with Apple
- [ ] CloudKit `Stamp` record: photo (CKAsset), lat/lng, createdAt, note, ownerID
- [ ] One-time migration: upload existing local stamps on first sign-in
- [ ] Sync new stamps on save; pull on launch / background
- [ ] UI: sync state (Backing up / Synced / Offline)
- [ ] Keep local cache for offline map
- [ ] Privacy policy (location + photos + iCloud); account deletion path

### Phase 2 — Share a stamp (no friend graph yet)

- [ ] Share sheet: stamped image + optional map snapshot, **or**
- [ ] Deep link / simple web view for one stamp

### Phase 3 — Connect friends (before or right after App Store)

- [ ] Invite via link or QR → accept → friendship
- [ ] Map toggle: Mine / Friends
- [ ] Stamp visibility: private | friends (default private or friends-only)
- [ ] Backend decision: CloudKit CKShare vs Firebase/Supabase for friend queries on map

## Deferred until after App Store

- Public discovery / nearby users
- Comments, likes, push notifications
- Cross-platform
- Monetization

## What I still don’t understand

- For “connect friend”: share one stamp only (A), friend list on map (B), or both (C)? — drives Phase 3 backend choice
- Whether Phase 3 is required before App Store or can ship backup + single-stamp share first
