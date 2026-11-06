# Manual QA Checklist

Use this checklist for the current static prototype. Record browser, device, date, tester, expected result, actual result, and evidence for each test. Do not mark a test passed without running it.

## 1. Initial load and navigation
- [ ] `index.html` loads without a blank screen or visible JavaScript error.
- [ ] Header navigation links scroll to the correct sections.
- [ ] Mobile menu opens, closes, and closes after a navigation selection.
- [ ] Workspace side navigation highlights the selected section.
- [ ] Mobile bottom navigation links reach the expected sections.

## 2. Strategy inputs
- [ ] Empty goal uses the documented fallback text.
- [ ] Entered goal, available time, budget, skills, and constraints appear in the generated draft.
- [ ] User-provided text is displayed as text, not interpreted as HTML.
- [ ] Generating a new plan replaces the task list as expected; confirm this behavior is understandable to users.

## 3. Execution tasks
- [ ] Add task using the button.
- [ ] Add task using Enter.
- [ ] Mark task complete and incomplete.
- [ ] Remove a task.
- [ ] Progress percentage and completed-task count update correctly.
- [ ] Empty state appears when there are no tasks.

## 4. Practice diary and chart
- [ ] Save a valid diary entry.
- [ ] Empty activity is rejected with a clear message.
- [ ] Saving another entry for the same date updates that date rather than duplicating it.
- [ ] Minutes are bounded to the expected range.
- [ ] Streak, total time, average score, history, and chart update.
- [ ] Chart range controls update the visible period.
- [ ] Refreshing the page clears in-memory tasks and diary entries; this is the current session-only behavior, not a persistence test failure.

## 5. Data portability
- [ ] Export creates a readable JSON file.
- [ ] Import restores profile fields, tasks, and diary entries.
- [ ] Invalid JSON and wrong application payloads are rejected without crashing.
- [ ] Missing or malformed individual fields do not break the page.
- [ ] Exported data is treated as personal data and stored safely by the user.

## 6. Review and sharing
- [ ] Strategy review renders all three review cards.
- [ ] Review output is clearly identified as local rule-based logic, not an AI model response.
- [ ] Copy, native share fallback, and image export work where supported.
- [ ] User-entered text is safely rendered in share preview.
- [ ] Sharing guidance warns users not to include sensitive information.

## 7. Localization and accessibility
- [ ] Korean, English, Chinese, and Japanese can be selected.
- [ ] Dynamic content generated after changing language is translated correctly.
- [ ] Form controls have usable labels or accessible names.
- [ ] Keyboard focus is visible and interactive controls are keyboard-operable.
- [ ] Text contrast and layout are usable at narrow viewport widths.
- [ ] Browser zoom at 200% does not hide essential controls.

## 8. Release checks
- [ ] Review the Git diff and ensure no credentials or private data are committed.
- [ ] Run all applicable checks on the proposed branch.
- [ ] Preview the Vercel deployment before merging.
- [ ] Confirm production deployment after an approved merge.
- [ ] Update product status only with evidence from completed tests.
