# Accessibility Check list

### Color

- [ ] Check the contrast for all normal-sized text. (Level AA compliance requires a contrast ratio of 4.5:1.)

- [ ] Check the contrast for all large-sized text. (Level AA compliance requires a contrast ratio of 3:1.)

- [ ] Check the contrast for all icons. ( Level AA compliance requires a contrast ratio of 3.0:1 )

- [ ] Check text that overlaps images or video.

- [ ] Check custom ::selection colors. (Is the color contrast you set in your ::selection CSS declaration sufficient? Otherwise someone may not be able read it if they highlight it.)

- [ ] Make sure to show emphasis by not only using the opposite color. (Use font-weight: bold or italic to emphasize.)

### Content

- [ ] Make sure that button, a, and label element content is unique and descriptive. ( Terms like “click here” and “read more” do not provide any context. )

### Code

- [ ] Don't disable zoom.
      People with partial vision and low vision enlarge text to make it more readable. Avoid user-scalable=”no”.

- [ ] Hide decorative elements with an aria attribute.

Decorative elements (that aren’t images) should be hidden with an aria attribute so assistive technology can ignore them.

### Images

- [ ] Make sure that all img elements have an alt attribute.

- [ ] Make sure that decorative images use null alt (empty) attribute values.

- [ ] For images containing text, make sure the alt description includes the image's text.

### Headings

- [ ] Use only one h1 element per page or view.

- [ ] The order of heading elements should descend, based on the “depth” of the content. For example, a h4 element should not appear on a page before the first h3 element declaration.

- [ ] Don't skip heading levels. For example, don't jump from a h2 to a h4, skipping a h3 element. If heading levels are being skipped for a specific visual treatment, use CSS classes instead.

### Keyboard Navigation

- [ ] Make sure there is a visible focus style for interactive elements that are navigated to via keyboard input.

- [ ] Check to see that keyboard focus order matches the visual layout. (for grids, check to see that the grid is in the correct order)

- [ ] Change the focus style, in order to show the user that the element is navigated to.

### Animation

- [ ] Ensure animations are subtle and do not flash too much.

- [ ] Provide a mechanism to pause background video. (Background video can be distracting, especially if content is placed over it.)

- [ ] Make sure all animation obeys the prefers-reduced-motion media query.

### Controls ( Controls are interactive elements such as links and buttons)

- [ ] Make sure all interactive elements have a visible focus style.
- [ ] Use the a element for links.
- [ ] Ensure that links are recognizable as links. (Color alone is not sufficient to indicate the presence of a link. Underlines are a popular and commonly-understood way to communicate the presence of link content.)

### Forms

- [ ] All inputs in a form are associated with a corresponding label element. ( Use a for/id pairing )
- [ ] Use fieldset and legend elements where appropriate.
- [ ] Make sure that form input errors are displayed in list above the form after submission.
- [ ] Make sure that error, warning, and success states are not visually communicated by just color. (People who are color blind, who have other low vision conditions, or different cultural understandings for color may not see the state change, or understand what kind of feedback the state represents if color is the only indicator.)

### Video

- [ ] Confirm the presence of captions. ( Captions allow a person who cannot hear the audio content of a video to still understand its content.)

### Media

- [ ] Make sure that media does not autoplay. (Autoplay is a bad user experience and Unexpected video and audio can be distracting and disruptive.)

- [ ] Check to see that all media can be paused.

### Fonts

- [ ] Use relative units for font sizes. (EM / REM / %)
- [ ] Increase text size to 200%. (Is the content still readable? Does increasing the text size cause content to overlap?)

### ARIA

Do rich, dynamic, web interfaces include ARIA markup ( IF NEEDED )
