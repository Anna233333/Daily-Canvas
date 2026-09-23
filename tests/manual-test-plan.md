# Daily Canvas manual test plan

## Core flow

- Open `code/index.html`; confirm the current day is selected.
- Submit an empty input; confirm no dot is created and an inline message appears.
- Enter “I am feeling down” and select **Paint**; confirm exactly one blue dot appears.
- Enter “I feel calm after a long walk”; confirm a green Calm suggestion and one new dot.
- Enter an unknown phrase; confirm the suggestion is Neutral.
- Choose a different palette color before painting; confirm the dot uses the chosen color.
- Refresh the page; confirm all dots retain their positions and appearances.

## Calendar and entries

- Select another day in the same month, add a moment, and confirm both days’ dots share the monthly canvas.
- Confirm the monthly moment list shows the date for every entry.
- Navigate to another month and confirm its canvas contains only that month’s entries.
- Navigate to the previous and next months.
- Confirm dates with entries show miniature colored dots.
- Select a painted dot; confirm its matching sentence is revealed in the moment list.
- Select **Edit** beside a moment; confirm an editor opens inside that moment row while the Paint composer remains unchanged.
- Change the sentence and select **Save**; confirm the existing entry updates without creating another dot or changing its color, date, or position.
- Select **Edit**, then **Cancel**, and confirm the saved entry is unchanged.
- Remove an entry and select **Undo** within three seconds; verify the same dot returns with its original text, color, date, and position.
- Confirm the visible **Undo** button accepts pointer and keyboard input while the toast is open.
- Remove an entry without selecting **Undo**; verify the action becomes permanent after three seconds.
- Remove two entries quickly; verify only the most recently removed entry remains undoable.

## Language rules

- “I am very happy” maps to Joy.
- “I am not happy” does not map to Joy solely because of “happy.”
- “I feel burned out” maps to Tiredness.
- “I feel bored” maps to Boredom rather than Neutral.
- “There is nothing to do” maps to Boredom.
- A sentence with equally strong keywords from two mood families falls back to Neutral.

## Personalization

- Add “jealous” with a custom green; confirm it appears in the palette and legend.
- Enter “I feel jealous”; confirm the new custom mood is suggested.
- Refresh the page; confirm the custom mood and color remain available.
- Change the color of a built-in mood; confirm its palette swatch, legend, and existing dots update.
- Try to add an existing keyword; confirm the app prevents the duplicate.

## Accessibility and layout

- Complete the write, color-select, paint, calendar, and remove flows using only a keyboard.
- Confirm focus indicators remain visible.
- Confirm each calendar date and paint dot has a useful screen-reader label.
- Test at desktop, tablet, and narrow mobile widths.
- Enable reduced motion and confirm dot and scroll animations are suppressed.
