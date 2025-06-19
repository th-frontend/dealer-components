# Customizing crawl-space Landing Page

This directory contains `index.html`, a landing page template for crawl space services. When adapting it for a new company, update the following items:

1. **Company Name and Contact Details**
   - Replace `[company]` tokens with the new company name (e.g., in the header logo link and introductory paragraphs).
   - Replace `[phone]`, `[display_addresses]`, and other company-specific tokens if they are not handled by your templating system.
2. **Service Area References**
   - Update `[state]` placeholders with the primary state served by the new company.
   - Modify any hard-coded references to "Michigan" or "Indiana" in the introductory text (around line 240) to reflect the correct service region.
   - Replace `[major cities 2]` with a comma-separated list of major service cities.
3. **External Links and Awards**
   - Update the BBB link and image alt text (lines ~45–46) to point to your company's profile instead of "Ayers Basement Systems".
   - Review the awards and badges images in the credibility section (lines 44–51). Swap them out if your company uses different graphics.
4. **Customer Review Section**
   - Remove or rewrite the customer review mentioning "Ayers" (line ~202) to showcase reviews for the new company.
5. **Images**
   - Replace any images that include the previous company's branding, such as `cs-ayers-lp3.jpg` (around line 400), with your own photographs.
   - Check other images for logos or text specific to the old company and update as needed.
6. **Company Logo**
   - The current SVG inside the header (lines 18–38) represents the existing logo. Replace it with your own company's SVG or image file.

Token placeholders in double brackets like `[[title]]` or `[[description]]` are managed by the internal system and typically do not need manual editing.
