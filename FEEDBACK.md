# Peer Feedback and Revision Record

## Review status

Peer review completed and the resulting improvements were committed on 16 November 2026.

## Reviewer

- **Name:** Classmate reviewer (name not provided)
- **Review date:** 16 November 2026
- **Page or figure reviewed:** Portfolio website project showcase, featured visualization and mobile layout

## Feedback received

The classmate found the README's explanation of the research question, data sources and methods clear, but recommended two improvements:

1. Add more explicit units to the chart and its explanation in the website's Project Showcase. Labels such as MOP, MOP million or percentage signs help non-specialist readers interpret a visualization correctly.
2. Improve the responsive layout because the navigation bar and chart container appeared slightly crowded or wrapped on a phone or other small screen.

## Improvements made

1. The featured figure caption now states that the chart uses **index points with January 2025 = 100**, and explicitly clarifies that the values are neither MOP nor percentages.
2. The narrow-screen CSS media query was refined. Navigation can now wrap cleanly, mobile spacing and type sizes are reduced, and the figure and project cards use smaller padding to prevent crowding on small screens.

## Corresponding commits

### Visualization unit clarification

- **Commit message:** Clarify visualization units after peer feedback
- **Commit hash:** `d341bad7e26fb1f500ef7e9642475c51dd9cd831`
- **Public commit URL:** https://github.com/vvvivianchen/cisc7204-macao-tourism-payments/commit/d341bad7e26fb1f500ef7e9642475c51dd9cd831

### Mobile layout improvement

- **Commit message:** Improve mobile layout after peer feedback
- **Commit hash:** `6b1eec200797bf64230bb4fb9dc5ee73e75e2706`
- **Public commit URL:** https://github.com/vvvivianchen/cisc7204-macao-tourism-payments/commit/6b1eec200797bf64230bb4fb9dc5ee73e75e2706

## Verification

- [x] The improvements directly respond to the recorded feedback.
- [x] Both changes have been committed to GitHub.
- [x] Both public commit URLs open the corresponding commits.
- [x] The updated page was checked in a local browser preview at desktop size.
- [ ] The deployed GitHub Pages URL will be tested in a signed-out browser after publication.
