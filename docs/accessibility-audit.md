Website Accessibility Audit Report

1. Objective

The objective of this audit is to evaluate the accessibility of a public-facing website using Google Lighthouse and keyboard-only navigation.

2. Testing Method

- Google Lighthouse accessibility audit
- Keyboard-only navigation
- Review of Lighthouse findings and relevant HTML evidence

3. Accessibility Findings

Issue 1: Incorrect ARIA Role Containment

Problem: Certain ARIA roles may not be contained within the required parent roles.

Impact: Screen readers may not interpret the page structure correctly.

Recommended Fix: Review the affected elements and use valid ARIA parent-child relationships.

Priority: Medium — confirm after reviewing the affected element.

Issue 2: Focusable Descendants Within an aria-hidden Element

Problem: Interactive elements may receive keyboard focus inside an element marked "aria-hidden="true"".

Impact: Keyboard and screen-reader users may encounter confusing navigation.

Recommended Fix: Ensure hidden content is not keyboard-focusable, or remove the conflicting hidden state when appropriate.

Priority: Medium — assess the affected element.

Issue 3: Insufficient Colour Contrast

Problem: Some foreground and background colour combinations may not provide sufficient contrast.

Impact: Text may be difficult for some users to read.

Recommended Fix: Adjust the colours to meet applicable WCAG contrast requirements.

Priority: Medium — assess the affected text and contrast ratio.

Issue 4: List Items Missing the Required Parent Element

Problem: Some list items may not be contained within an appropriate parent element.

Impact: Screen readers may not announce the list structure correctly.

Recommended Fix: Use appropriate list markup, such as "<ul>" or "<ol>", where applicable.

Priority: Medium — verify the affected HTML.

Issue 5: Document Does Not Have a Main Landmark

Problem: The page may not provide a main landmark for its primary content.

Impact: Screen-reader users may have difficulty navigating directly to the main content.

Recommended Fix: Identify the primary page content using an appropriate "<main>" element or main landmark.

Priority: Medium — assess the page structure.

4. Evidence

Screenshots of the Lighthouse findings are collected separately. Each screenshot should be matched to its corresponding issue.

5. Conclusion

The audit identified five potential accessibility issues. The findings should be verified against the affected elements, corrected where necessary, and retested using Lighthouse and keyboard navigation.
