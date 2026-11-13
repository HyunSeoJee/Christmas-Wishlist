# Christmas Wishlist: MVP Requirements

## Problem
People want to build a Christmas wishlist and share it with family and friends without it being tied to one store.

## Users
- **List owner:** has an account, creates and manages list.
- **Viewer:** receives a link, views the list. No account needed.

## User Stories & Acceptance Criteria

### 1. Accounts
As a visitor, I want to create an account and log in so that my
lists are saved and private to me.
- [ ] I can register with username + password
- [ ] Duplicate usernames are rejected with a clear message
- [ ] Passwords are stored hashed, never in plain text
- [ ] I can log in and log out
- [ ] Logged-out users cannot edit anything

### 2. Add items manually
As an owner, I want to add items by hand so that I can include
anything I want.
- [ ] An item has: name (required),
      link (optional), image URL (optional), notes (optional)
- [ ] I can edit and delete items
- [ ] Items display as cards in a grid ("block icon view")

### 3. Share a link
As an owner, I want a shareable link so that others can view my list.
- [ ] Anyone with the link can view the list (read-only)
- [ ] Viewers cannot edit anything

## Out of Scope (v2+)
- Importing items from product URLs
- Claiming / "I'm buying this" feature when logged in
- Claiming feature is not viewable to list owner
- Social login, password reset, email verification

## Decisions
- Viewers don't need an account. Decision: yes.
- Currency: single currency (USD) for now.
- Images: store the URL only, don't upload files.