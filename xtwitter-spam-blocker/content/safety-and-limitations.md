---
title: "Safety and Limitations"
description: "Review the product boundaries, detection limitations, local hiding behavior, and safety expectations."
weight: 50
---

# Safety and Limitations

X/Twitter Spam Blocker is designed to reduce matching spam while keeping important account actions under user control. This page explains what the extension can do, what it cannot guarantee, and how to use it safely.

## Review Before Blocking

Blocking an account can be an important action, so the extension does not silently block detected accounts in the background.

When block review is enabled, high-risk accounts are shown in a floating review panel on X/Twitter. You choose which accounts to block, and the extension only submits selected accounts to X/Twitter after you confirm.

## Local Hiding Is Not Deletion

When the extension hides matching content, it changes your local browsing experience. It does not delete the original tweet, remove the content from X/Twitter, or affect what other users see.

If you disable the extension or browse from another device without the extension, the original content may still be visible.

## Detection Is Not Perfect

The current version uses rule-based matching for adult-spam replies, off-platform lure patterns, unwanted promotional replies, and related high-risk profile signals.

These rules can help reduce common spam, but they cannot guarantee complete detection. Some spam may not be hidden, and some matching content may need review to avoid mistakes.

## Current Scope

The extension is focused on a specific spam problem: repetitive adult-spam replies, suspicious lure patterns, unwanted promotional replies, and high-risk accounts that frequently appear in X/Twitter browsing.

It is not a full trust and safety system, a complete bot detector, a complete scam detector, or a replacement for X/Twitter's own safety tools.

## X/Twitter Changes May Affect Behavior

X/Twitter can change page structure, APIs, request behavior, or visible content formats at any time. Those changes may temporarily affect spam detection, hiding, review, dashboard statistics, or blocking behavior.

If something stops working, check for extension updates or contact support with the extension version, browser version, and a short description of the affected page.

## Use Caution With Blocking

Before confirming a batch block, review the account list. Do not block accounts only because they appeared in the panel if you are unsure.

The review step exists so you can make the final decision.

## Handling Mistakes

If content is hidden by mistake, remember that local hiding is not deletion. The original content still exists on X/Twitter, and it may still be visible if you turn off filtering in Settings, disable the extension, or browse from another device without the extension.

If an account appears in the floating review panel by mistake, leave it unchecked. The extension will not block that account unless you select it and confirm the block action.

If you already confirmed and completed a block, you can use the Activity Log to find it. Filter for blocked account records, locate the related account, click the ScreenName link to open the user's X/Twitter profile, and manually unblock the account on X/Twitter.

## Data Handling Boundaries

In the current version, extension settings, statistics, activity history, and daily block safety status are stored locally on your device.

The extension does not send tweet content, account content, activity history, or protection statistics to our servers in the current version. If a future version adds optional spam reporting, the privacy policy and product documentation will be updated before release.

## Independent Product

X/Twitter Spam Blocker is an independent browser extension and is not affiliated with, endorsed by, or sponsored by X Corp. or Twitter.
