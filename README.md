# Triple Peaks Coffee Shop

This is the second project of the Software Engineering program at TripleTen. It was created using HTML and CSS, based on the design brief.

## Project features

- Semantic HTML5
- Flexbox
- Positioning
- Flat BEM file structure
- A custom form
- CSS animation and transform

## Plan on improving the project

- Add a custom focus ring style around the form submit button. The browser's default focus ring doesn't have sufficient color contrast against the blue button background color. This means keyboard users could have difficulty figuring out whether they're focused on the button.

These CSS styles could be used to create a custom focus ring around the button that's visible on key focus:

```css
.form__button:focus-visible {
  outline: 2px solid #1878dc;
  outline-offset: 3px;
}
```

- Add parameters for captions in the YouTube iframe URLs, and include video transcripts (either in a text document link or linked out to a separate page). Captions and transcripts are helpful for users who are unable or have difficulty listening to the videos.

YouTube lists parameters that can be used with iframe URLs here: [YouTube Embedded Players and Player Parameters]https://developers.google.com/youtube/player_parameters cc_load_policy (set to 1) is the correct parameter for ensuring closed captions added to the video would be turned on by default. Would also consider adding the rel parameter (set to 0) to show related channel videos when users pause or reach the end of the video, instead of the random video assortment that's usually shown.

- Create a reduced motion preference for the pulsate animation in the About section. This would remove or reduce the amount of motion when a user has enabled reduced motion settings on their device. The pulsing animation could be potentially triggering to someone sensitive to motion or flashing-like movement. MDN outlines documentation for reduced motion settings here: [prefers-reduced-motion]https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-reduced-motion
