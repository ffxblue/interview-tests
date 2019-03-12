---
layout: test
title:  WordPress Metabox
---

## Summary

The purpose of this exercise is for us to get a sense of how you would approach designing and implementing a simple WordPress integration before we get you in for an interview. We're avoiding tricky algorithmic tests in favor of something that shows how you approach problems and organise a codebase.

There is no time limit for this test, but we expect most applicants to complete the requirements in roughly 3-4 hours.

If you make any assumptions about requirements, or use any online resources to solve a problem, please make note of these in your code comments.

Your solution will be evaluated internally by your potential co-workers. You should expect a response from us within two business days.

## User story

> As a editor or journalist\
I can access advertising features in a single location\
So I can easily find all advertising-related settings

## Acceptance criteria

- A new metabox is registered for the standard "post" post type.
- The metabox title is "Advertising Settings".
- Three fields appear in the metabox.
- A "Save" button appears in the metabox.

### Advertisements field

- The advertisements field has:
  - The label "Advertisements:".
  - Two inline radio inputs with labels: "Off" and "On".
  - The "On" radio input selected by default.

### Commercial content type field

- The commercial content type field has:
  - The label "Commercial content type:".
  - Four inline radio inputs with labels: "None", "Sponsored content", "Partnered content" and "Brought to you by".
  - The "None" radio input selected by default.

### Advertiser name field

- The advertiser name field has:
  - The label "Advertiser name:".
  - A text input.
- The advertiser name field is hidden while "None" is the selected commercial content type.

### Save button

- A save button appears at the botton of the metabox.
- When clicked, a request is sent to WordPress to save the current metabox field values to post meta for the current post.

## Bonus

The following tasks are not required, but nice to have:

1. Test WordPress environment to be hosted and publicly accessible (with username/password)

## Environment

Our environment is set up as per below. You don't need to use this exact environment but the closer the better.

- WordPress 4.9.8.
- PHP 7+.
- Webpack.
- ES2015 via Babel compilation.
- Sass.

Additionally, we only the support the most recent versions of Google Chrome.

## Deliverables

All acceptance criteria should be met (to best of ability and time available). A link to your repo should be sent to: `amp HYPHEN tech HYPHEN test HYPHEN submissions HYPHEN group AT fairfaxmedia DOT com DOT au`
