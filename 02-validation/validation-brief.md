# Validation Brief

> Module 2 · Validation. Frame the riskiest assumption, then build to test it. **This locks your scenario, no switching after M2.**

## Scenario

Self service landing page tool for marketing (own product)

## Riskiest assumption

_The one belief that, if false, sinks the idea._

Marketing managers can self service their own short content for landing pages

## Hypothesis

> We believe **the manual work web team does to intake lp content and design** will cause **too show and fustrates stakeholders** for **PMM and marketing (supports web team)**. We'll know we're right when **output that passes muster with web design/UX**.

## Risk type

- [ ] Value (do they want it?)
- [x] Usability (can they use it?)
- [ ] Feasibility (can we build it?)
- [x] Viability (should we?)

## Kill switch

_The result that would make you stop or pivot._

output does not meet web design standards (as judged by web design team)

## The three ingredients

- **Real data (domain metrics):** _____
- **User voice (verbatim quotes):** _____
- **Hypothesis (above):** ✓

## Here is my final prompt. I modified.
Build a high-fidelity, clickable prototype for Self service landing page tool for marketing that tests one hypothesis, not just a nicer-looking screen.
Hypothesis: we believe the manual work web team does to intake lp content and design will cause too slow and frustrates stakeholders for PMM and marketing. But right now the web team is spending a huge amount of time processing and managing requests for what is basically some content on the left and design on the right.  We'll know we're right when marketing select a template and develop their own content that can be input into a template and that output passes muster with web design/UX.
Ground it in real context. Put these ON SCREEN as real content, not placeholders:
Make the kill switch observable in the UI: output does not meet web design standards (as judged by web design team)
Match a clean, credible visual reference (I'll attach a screenshot, copy the pattern, not the brand). Build only the core screens that would prove or break the hypothesis.
What this prototype should do:
1. Create three fixed landing-page templates.
   Base them on https://www.arc.io/builders-fund, using the design system of https://www.arc.io.
   Create three distinct, general-purpose layouts. Do not assign them to specific campaign types. All three must keep text on the left and a form on the right.
   These layouts are fixed: users can choose a template and edit its content, but cannot rearrange sections, change colors, or modify the layout. The templates do not change over time.
   Use a consistent, fixed color palette derived from the references. The tool’s interface should feel polished and credible; the landing-page previews should retain a clean wireframe appearance.
   The right-side form must contain these default fields:
   - Name
   - Company name
   - Phone number
   - Company size
   - Submit button
   This landing-page form is for visual demonstration only. It does not collect or submit data.
   Include image areas only where they support good UX. Image areas start as gray wireframe placeholders. Users can replace them with real uploaded images.
2. Start with an intake screen.
   Ask for:
   - Name
   - Email
   - Department
   - Campaign name or description
   - Campaign goal
   - Target audience
   - Primary message or offer
   Use the intake answers to inform the template recommendation and carry the information through the demo. Keep this screen concise.
3. Show the three templates and recommend one.
   After intake, display previews of all three fixed layouts.
   Recommend one using simple, consistent rules based on the intake answers. Explain the recommendation in a short, plain-language sentence.
   Users can accept the recommendation or select either of the other two templates. Show enough detail in each preview to make the differences clear.
4. Let users enter and edit content directly in the selected template.
   Users click text in the landing-page preview to edit it in place. Provide clear cues showing which text is editable.
   Define sensible character limits for each editable field in each template, based on readability and available space. Disclose each limit and show a live character counter.
   Allow users to exceed a limit while drafting, but:
   - Clearly flag the affected field.
   - Explain how many characters must be removed.
   - Require users to shorten all over-limit content before moving to approval.
   - Apply the same validation to PDF export when that feature is implemented.
   For templates with an image area, support uploading, displaying, and replacing a real image.
   Include a disabled “Import from Google Docs — Coming later” button. Do not implement Google Doc import in this version. Users must enter text themselves.
   Keep the default form on the right. Support for populating it from a form ID is a future feature.
5. Provide a preview of the completed landing page.
   Let users review their content and uploaded image in the selected layout, then return to editing.
   Include:
   - A disabled “Export PDF — Coming later” button. PDF generation is outside this demo’s scope.
   - A “Save to workspace” demo control. It may show a clearly labeled simulated saved state, but must not claim the content is persistently stored.
   Real workspace storage and returning in a later session will be built later. Preserve edits while navigating between screens during the current demo session.
6. End at the approval handoff button.
   Show a “Submit for web approval” button with a nearby note explaining that submission is not implemented in this demo.
   Keep the button disabled while any text exceeds its character limit. Once the content meets the limits, the button may be enabled, but clicking it must not send data, navigate to an approval workflow, or claim successful submission. The prototype ends here.
   Display the intake information alongside the final preview so the intended handoff package is visible.
   Make the design acceptance criterion observable on screen:
   - Approval status: Not yet reviewed by the web design team.
   - Design acceptance criterion: Output must meet web design standards, as judged by the web design team.
   - Kill switch: Output does not meet web design standards.
   Present the kill switch as a criterion for evaluating the hypothesis, not as a judgment that the system has already made. Do not build designer approval controls or automated design approval.
   In a future version, submission will send the intake information and a link to the created wireframe to the web team.
7. Keep the remaining workflow out of scope.
   Future functionality includes:
   - Google Doc import and automatic placement of imported content into template fields.
   - PDF export.
   - Persistent workspace saving and reopening.
   - Actual submission and review by the web team.
   - Web team approval, design image updates, and publishing to the web content management system.
   For this demo, make the core flow functional: intake → template recommendation and selection → direct text editing and image upload → final preview → approval handoff button.
   The prototype should let us test whether marketing users can independently create a landing-page draft within fixed layouts and content limits, and let the web design team assess the resulting draft against its standards.
