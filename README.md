# Contribution 1: Create an Acknowledgements section for the README

**Contribution Number:** 1
**Student:** Monica Gnajewski  
**Issue:** https://github.com/InsightSoftwareConsortium/ITK/issues/454
**Status:** Phase III Complete

---

## Why I Chose This Issue

I chose this issue to get a good grasp of how to start contributing to an open source codebase. I thought it was simple enough to work on without feeling frustrated or defeated. I also thought it was suprising to see that these kind of simple requests happen in large-scale projects. 
With my contribution, I hope to become more accustomed to working on a public codebase and collaborating with other maintainers. I beleive these skills would be relevant in the working field where you have to edit and remove bugs in code written by many different people.

---

## Understanding the Issue

### Problem Description
The ITK README.md does not have a dedicated Acknowledgements section. The maintainer requested adding one to acknowledge organizations like the National Library of Medicine, grants, and other entities that have funded ITK development over the years.

### Expected Behavior
The README contains a clearly labeled "Acknowledgements" section that consolidates and credits the project's funders and sponsoring organizations (e.g., the National Library of Medicine, relevant NIH grants, NumFOCUS, and the Insight Software Consortium).

### Current Behavior
There is no standalone Acknowledgements section. Funding and sponsorship information is only mentioned in passing within the existing README prose (e.g., a brief note that ITK is fiscally sponsored by NumFOCUS), so the funders are not acknowledged in one clear, dedicated place.

### Affected Components
README.md in the ITK repository.

---

## Reproduction Process

### Environment Setup
To set up my local environment, I had to fork the repo and clone my fork.

### Steps to Reproduce
1. Open the current README.md on the main branch of InsightSoftwareConsortium/ITK.
2. Search the file for an "Acknowledgements" heading.
3. Notice no dedicated Acknowledgements section exists; funding/sponsor references appear only inline in the prose.

### Reproduction Evidence

- **Commit showing reproduction:** https://github.com/InsightSoftwareConsortium/ITK/commit/d4f2cfe34885ff2b5378d752cbf3958a41414e98
- **My findings:** Found that there was no "Acknowledgements" section.

---

## Solution Approach

### Analysis
The root cause is that the section was never written. The maintainer and other contributors have pointed to source material in the issue thread (NLM project pages, ITK funding history, and NumFOCUS-related PRs), so the work is gathering that information and presenting it as a dedicated section.

### Proposed Solution
Add a new Acknowledgements section near the bottom of README.md that credits the funding organizations and sponsors of ITK, drawing on the references linked in the issue discussion.

### Implementation Plan
- Review the resources linked in issue #454 (NLM project pages, ITK funding history) and the nipype funding-acknowledgement section a maintainer cited as a model.
- Identify the organizations and sponsors to credit: the National Library of Medicine, relevant NIH grants, NumFOCUS (fiscal sponsor), and the Insight Software Consortium.
- Add a new ## Acknowledgements section near the bottom of README.md consolidating this information into one clear, readable section.
- Verify the Markdown renders correctly and any links resolve.
- Follow ITK's DOC: commit-message convention and contribution guidelines.

**Understand:** ITK's README lacks a dedicated section acknowledging its funders (NLM, grants, NumFOCUS, ISC); the goal is to add one.

**Match:** There is an inline NumFOCUS sponsorship note already in the README, but no Acknowledgements section.


**Plan:**
1. Review the resources linked in issue #454 to identify the organizations and grants to credit.
2. Draft an Acknowledgements section consolidating that information.
3. Add the section to README.md and verify Markdown rendering.

**Implement:** [Link to your branch/commits as you work]

**Review:** I will make sure I am following the project's contribution guidelines.

**Evaluate:** I will preview the rendered Markdown, and confirm links resolve.

---

## Testing Strategy
This is a documentation-only contribution and changes no source code. ITK's automated test suite does not cover README prose, so validation is manual rather than test-driven.

### Unit Tests
N/A since no code paths are added or modified, so there is nothing for unit tests to exercise. 

### Integration Tests
N/A since the change does not interact with any build, module, or runtime behavior.

### Manual Testing

- **Markdown rendering:** Previewed `README.md` on GitHub (and locally) to confirm the new section renders correctly with proper heading level, paragraph breaks, and list formatting, and that it sits cleanly between the existing sections.
- **Link verification:** Clicked every link in the new section to confirm each resolves and none returns a 404.
- **Pre-commit hooks:** Ran ITK's pre-commit hooks, which check commit-message format and line length; the `DOC:` commit and the wrapped section body pass.
- **Scoped diff:** Confirmed `git diff` touches only `README.md`, with no stray whitespace or unrelated changes.

---

## Implementation Notes

### Week 2 Progress
Researched ITK's funding history using the resources linked in issue #454 (the NLM project page, ITK's About/history pages) plus the founding-contract details from ITK's own documentation. Drafted and added a new `## Acknowledgements` section to `README.md` covering:
- ITK's 1999 origin under a US National Library of Medicine (NLM) / NIH contract in support of the Visible Human Project, directed by NLM project manager Dr. Terry Yoo.
- The six founding Insight Software Consortium contractors (GE Corporate R&D, Kitware, MathSoft/Insightful, UNC, the University of Tennessee, and UPenn).
- Ongoing funding sources (predominantly NLM, plus other NIH institutes, the NSF, and the US Department of Defense TATRC).
- ITK's current fiscal sponsorship by NumFOCUS.

### Code Changes

- **Files modified:** `README.md`
- **Key commits:** [link]
- **Approach decisions:**
  - Placed the section after `## Professional Services` and before `## Citation` to group it with the other project/backer context.
  - Acknowledged funders at the organization/agency level, consistent with what's verifiable from the sources in issue #454.
  - Followed ITK's commit conventions.

---

## Pull Request

**PR Link:** [GitHub PR URL when submitted]

**PR Description:** [Draft or final PR description - much of the content above can be adapted]

**Maintainer Feedback:**
- [Date]: [Summary of feedback received]
- [Date]: [How you addressed it]

**Status:** [Awaiting review / Iterating / Approved / Merged]

---

## Learnings & Reflections

### Technical Skills Gained

[What you learned technically]

### Challenges Overcome

[What was hard and how you solved it]

### What I'd Do Differently Next Time

[Reflection on your process]

---

## Resources Used

- [Link to helpful documentation]
- [Tutorial or Stack Overflow post that helped]
- [GitHub issues or discussions that helped]
