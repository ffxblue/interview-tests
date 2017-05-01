---
layout: test
title:  WordPress Categories
---

## Summary

The purpose of this exercise is for us to get a sense of how you would approach designing and implementing a simple WordPress integration before we get you in for an interview. We're avoiding tricky algorithmic tests in favor of something that shows how you approach problems and organise a codebase.

There is no time limit for this test, but we expect most applicants to complete the requirements in roughly 2-3 hours.

Feel free to use any PHP framework you like, but note that submissions utilising WordPress will be looked on favourably.

If you make any assumptions about requirements, or use any online resources to solve a problem, please make note of these in your code comments.

Your solution will be evaluated internally by your potential co-workers. You should expect a response from us within two business days.

## User story

> As a WordPress system  
I want to get all categories from an external API  
So that a single system handles taxonomy and their relationships

## Acceptance criteria

1. WordPress polls a fake API (see dev notes below) every 30 minutes to check for changes to categories
1. Any change to categories in the API should be reflected in WordPress
1. The hierarchy of categories should be maintained (i.e. parent/child relationship)
1. Add 'Update categories now' button to Settings/General in the WordPress admin interface that will update categories on demand
1. Code for the above to be available via GitHub or BitBucket repo
1. Repo should have README.md that contains the following:
  - Any project quirks or setup notes
  - Any work left in progress
  - A short paragraph outlining what you thought of the test
  - How long the test took to complete

## Bonus

The following tasks are not required, but nice to have:
1. Test WordPress environment to be hosted and publicly accessible (with username/password)
1. Disable ability to add new categories from within WordPress

## Dev notes

You can create a fake REST API with [JSON Server](https://github.com/typicode/json-server).

**Example db.json:**
```json
{
  "categories": [
    {
      "id": 1000,
      "name": "State",
      "parent_id": null
    },
    {
      "id": 1001,
      "name": "NSW",
      "parent_id": 1000
    },
    {
      "id": 1002,
      "name": "VIC",
      "parent_id": 1000
    },
    {
      "id": 1003,
      "name": "QLD",
      "parent_id": 1000
    },
    {
      "id": 1004,
      "name": "WA",
      "parent_id": 1000
    },
    {
      "id": 1005,
      "name": "ACT",
      "parent_id": 1000
    },
    {
      "id": 1006,
      "name": "National",
      "parent_id": null
    },
    {
      "id": 1007,
      "name": "World",
      "parent_id": null
    }
  ]
}
```

## Deliverables

All acceptance criteria should be met, to best of ability and time available. A link to your repo should be sent to: `blueco DOT tech DOT test AT gmail DOT com`
