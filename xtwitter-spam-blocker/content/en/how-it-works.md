---
title: "How It Works"
description: "Understand how X/Twitter Spam Blocker filters X/Twitter responses, matches spam signals, and separates hidden content from block review."
weight: 30
---

# How X/Twitter Spam Blocker Works

X/Twitter Spam Blocker filters supported X/Twitter responses before they are rendered in your browser. It parses tweets and user profile data from those responses, matches spam signals, and then decides whether matching content should be hidden or sent to block review.

## Inline Response Filtering

When X/Twitter loads supported timelines, notifications, tweet details, search results, bookmarks, or user tweet views, the extension processes the response inline before the page renders it.

From that response, the extension reads the tweet content, author profile fields, links, and related metadata needed for spam filtering. The page then receives a filtered response, so removed items do not appear in the local browsing view.

## Rule-Based Matching

The extension uses rule-based matching across multiple tweet and user signals. A decision can consider signals such as reply text, external links, profile descriptions, profile URLs, account metadata, and repeated high-risk patterns.

This lets the extension separate lower-risk content cleanup from higher-risk account handling. A tweet may be removed from your local view, while a stronger match involving both tweet behavior and account profile signals can create a block-review candidate.

## Hide and Block Review

The extension uses two main filtering outcomes:

`hide` removes matching content from the response before X/Twitter renders it. The content disappears from your local browsing view, and the action can be recorded in the Activity Log.

`block review` removes the matching content from the response and also creates a review candidate for the account. The account appears in the floating review panel, where you can decide whether to block it.

Candidates are not automatically blocked. A block action is only submitted after you select accounts in the review panel and confirm the action.

## Local Records

The extension stores local records used by the dashboard, Activity Log, settings, and safety limits. These records can include:

- Protection statistics.
- Hidden content records.
- High-risk account candidates.
- Successful block actions.
- Failed block attempts.
- Daily block safety status.

In the current version, settings, statistics, activity history, and safety status are stored on your device.

## Network and Permission Boundary

The extension needs access to supported X/Twitter pages to process responses, remove matching content from the local rendered view, show the floating review panel, and perform block actions that you confirm.

Access to `abs.twimg.com` is used only to read X web assets needed to prepare request verification values for confirmed block requests.

## No Remote Code Execution

All extension JavaScript is packaged with the extension. The extension does not load or execute remote JavaScript or WebAssembly, does not inject external script files, and does not evaluate remotely fetched code.

## What It Does Not Do

X/Twitter Spam Blocker does not replace X/Twitter's own safety systems. It does not guarantee detection of all spam, scams, bots, or abusive content. It is designed as a focused browsing cleanup tool with user-reviewed blocking.
