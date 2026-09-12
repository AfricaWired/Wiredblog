---
title: "What We Look For Before Adding a Dependency"
category: "Cybersecurity"
author: "AfricaWired Team"
date: 2026-08-21 09:00:00 +0300
---
Every third-party package we pull into a project is code we did not write running with the same access as the code we did. Before adding one, we check who maintains it, how recently it has been updated, how large its own dependency tree is, and whether it has a history of unresolved security advisories.

None of those checks are exotic — they take a few minutes — but skipping them is how supply-chain risk quietly accumulates in a codebase over a few years of "just add the package that solves this quickly."

Dependencies already in use are re-checked on the same schedule as the rest of our security reviews, not just at the moment they are added.
