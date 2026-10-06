# CampaignFlow AI

CampaignFlow is an interactive product prototype for turning one campaign brief into coordinated drafts for multiple content formats while preserving a clear human review and approval process.

## Live Demo

[Open CampaignFlow AI](https://campaignflow-rodrigo.rodriikndr2003.chatgpt.site)

## The Problem

Creating content for several channels is only one part of campaign execution. Teams also need to understand which version was reviewed, what changed after approval, and which content is ready to be used.

CampaignFlow explores a workflow that makes those states visible rather than treating content generation as the final step.

## Product Flow

1. Enter a campaign brief.
2. Generate template-based drafts for four content formats.
3. Review and edit each draft.
4. Save changes in the revision history.
5. Approve content that is ready.
6. Export only the latest approved drafts.

## Key Product Decision

Approval belongs to a specific revision, not to the document in general.

If a user edits approved content, CampaignFlow automatically returns that draft to “In review.” This prevents a newly edited version from appearing approved when only the previous version was reviewed.

The prototype follows four related rules:

- Every saved edit creates or updates a visible revision.
- Approval applies only to the revision that was reviewed.
- Editing approved content returns the draft to “In review.”
- Export includes only the latest approved revisions.

## What I Built and Improved

I defined the product problem, workflow, review states, approval rules, failure cases, and testing scenarios. I first represented the concept in Canva and then developed it into an interactive web prototype using AI-assisted development and template-based content generation.

The prototype includes:

- A structured campaign brief
- Four content-format drafts
- Editable content
- Revision history
- Review and approval states
- Browser-local saving
- Approved-only export

## How I Checked the Workflow

I used a repeatable failure-case walkthrough:

1. Approve a draft.
2. Modify the approved content.
3. Confirm that the draft returns to “In review.”
4. Attempt to export the campaign.
5. Verify that the edited draft remains excluded until it is approved again.

## Current Limitations

CampaignFlow is an early product prototype rather than a production application.

- Content generation is template-based and does not currently use a live LLM.
- Data is stored locally in the browser.
- The prototype is single-user.
- It does not publish content to external platforms.
- It has not yet been validated with external marketing teams or real collaborative usage.

## Next Steps

The next stage would be to conduct usability sessions with potential users and measure:

- Whether users understand the review states without instruction
- Whether revision history helps reviewers identify changes
- Whether approved-only export reduces workflow errors
- How long it takes to move a campaign from brief to approved deliverables

## AI Assistance Disclosure

I developed the product reasoning, workflow, approval model, examples, and testing scenarios. I used ChatGPT and ChatGPT Sites to assist with implementation, structure, and English-language editing. No real user research, production integrations, or model capabilities are represented where they do not exist.

## Creator

**Rodrigo Fernández Martínez**  
Business Administration – Marketing, University of the Pacific
