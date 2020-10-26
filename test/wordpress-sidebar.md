---
layout: test
title:  Gutenberg Sidebar
---

## Summary

The purpose of this exercise is for us to get a sense of how you would approach designing and implementing a simple WordPress integration before we get you in for an interview. We're avoiding tricky algorithmic tests in favor of something that shows how you approach problems and organise a codebase.

There is no time limit for this test, but we expect most applicants to complete the requirements in roughly 3-4 hours.

If you make any assumptions about requirements, or use any online resources to solve a problem, please make note of these in your code comments.

Your solution will be evaluated internally by your potential co-workers. You should expect a response from us within two business days.

## User story

> As a editor or journalist  
I can access advertising features in a single location  
So I can easily find all advertising-related settings

## Acceptance criteria

1. In the Gutenberg/Block Editor, a new custom panel is visible in the sidebar for the standard "post" type
1. The custom panel title is "Advertising Settings"
1. Three fields appear in the custom panel, their requirements are outlined below
1. These fields should be disabled while post is being saved/updated/published
1. These fields have unit tests

### Field 1: Advertisements

- Label: "Advertisements"
- Type: Toggle control
- Default: On/True

### Field 2: Commercial content type

- Label: "Commercial content type"
- Type: Radio control
- Options: "None", "Sponsored content", "Partnered content" and "Brought to you by"
- Default: "None"

### Field 3: Advertiser name

- Label: "Advertiser name"
- Type: Text control
- Visibility: The advertiser name field is hidden while "None" is the selected commercial content type

## Bonus

The following tasks are not required, but nice to have:

- Test WordPress environment to be hosted and publicly accessible (with username/password)
- Local environment is ideally run via Docker
- Frontend code is ideally Typescript
- Custom panel has functional tests

## Deliverables

All acceptance criteria should be met (to best of ability and time available). A link to your repo should be sent to: `amp HYPHEN tech HYPHEN test HYPHEN submissions HYPHEN group AT fairfaxmedia DOT com DOT au`
