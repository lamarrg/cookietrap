# DomainGuard

A Firefox extension that shows you what data websites store on your browser — and lets you delete it.

## What it does

- **See what sites store** — View cookies, localStorage, and sessionStorage for any site you visit, right from your browser sidebar
- **Delete data on demand** — Remove individual items or clear everything a site has stored with one click
- **Auto-delete on leave** — Turn on "delete on leave" for any domain, and DomainGuard wipes its data when you close the last tab for that site
- **Spot third-party trackers** — See which third-party domains are setting cookies as you browse, and where they came from

## How to install

DomainGuard isn't on the Firefox Add-ons store yet, so you'll load it as a temporary add-on:

1. Clone or download this repository
2. Open Firefox and go to `about:debugging#/runtime/this-firefox`
3. Click **Load Temporary Add-on...**
4. Select any file in the repository folder (e.g., `manifest.json`)
5. DomainGuard's icon appears in your toolbar — you're ready to go

No build step needed. The extension runs directly from the source files.

> **Note:** Temporary add-ons are removed when you close Firefox. You'll need to re-load it each session until a signed version is available.

## What to expect

**Opening the panel** — Click the DomainGuard icon in your toolbar. You'll get two options:

- **Open in sidebar** — Shows the panel docked to the side of your browser window
- **Open in window** — Opens a detached panel you can position anywhere

**The panel has two sections:**

1. **This domain** — Shows all cookies, localStorage, and sessionStorage items for the site in your active tab. You can delete items individually or clear them all. The "delete on leave" toggle lets you auto-clear this domain's data when you close all its tabs.

2. **Third-party data** — Lists third-party tracking cookies observed across all the sites you've visited, along with which sites triggered them. You can delete these individually or clear them all at once.

The panel updates automatically as you switch tabs and as data changes.

## Current status

DomainGuard is in active development. All core features are implemented and working. It is not yet available on the Firefox Add-ons store.

Firefox only (Manifest V2).
