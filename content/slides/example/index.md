---
title: Slides
summary: An introduction to using Academic's Slides feature.
authors: []
tags: []
categories: []
date: "2019-02-05T00:00:00Z"
slides:
  # Choose a theme from https://github.com/hakimel/reveal.js#theming
  theme: black
  # Choose a code highlighting style (if highlighting enabled in `params.toml`)
  #   Light style: github. Dark style: dracula (default).
  highlight_style: dracula
---

# Create slides in Markdown with Academic

[Academic](https://sourcethemes.com/academic/) | [Documentation](https://sourcethemes.com/academic/docs/managing-content/#create-slides)

---

{{< slide id="hello" background="#FFF" background-image="https://www.dropbox.com/s/wizg1tmov3f3g7r/singer.jpg?raw=1" transition="zoom" transition-speed="fast" >}}

## Features 

- Efficiently write slides in Markdown
- 3-in-1: Create, Present, and Publish your slides
- Supports speaker notes
- Mobile friendly slides

{{% speaker_note %}}

Thsi is a test.

{{% /speaker_note %}}

---

### Test 

<span class="smallish">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed feugiat nisi nec ante porttitor finibus. Donec at quam a mauris tristique sodales. Praesent fringilla nisl et vulputate lacinia. Aliquam in nunc fermentum, mollis metus eu, rhoncus metus. Sed nibh sem, egestas sed pellentesque nec, pulvinar id augue. Proin venenatis sodales sem, in commodo leo volutpat eget. Quisque quis aliquet diam. Aliquam sodales eu ipsum ac accumsan. Fusce at dolor quis leo aliquet pretium. Duis malesuada imperdiet neque quis scelerisque. Pellentesque aliquam hendrerit lectus id dictum. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Phasellus faucibus facilisis pellentesque. Nulla nec erat id purus congue sollicitudin eget nec nisl. Morbi viverra blandit aliquet. Pellentesque sollicitudin neque ut odio hendrerit, at cursus tellus bibendum. Nam at sodales nulla. Nulla elementum pharetra sem sit amet sodales. Phasellus non magna aliquam, vehicula sem eget, congue libero. </span>

---

## Controls

- Next: `Right Arrow` or `Space`
- Previous: `Left Arrow`
- Start: `Home`
- Finish: `End`
- Overview: `Esc`
- Speaker notes: `S`
- Fullscreen: `F`
- Zoom: `Alt + Click`
- [PDF Export](https://github.com/hakimel/reveal.js#pdf-export): `E`

---

## Code Highlighting

Inline code: `variable`

Code block:
```python
porridge = "blueberry"
if porridge == "blueberry":
    print("Eating...")
```

---

## Math

In-line math: $x + y = z$

Block math:

$$
f\left( x \right) = \;\frac{{2\left( {x + 4} \right)\left( {x - 4} \right)}}{{\left( {x + 4} \right)\left( {x + 1} \right)}}
$$

---

## Fragments

Make content appear incrementally

```
{{%/* fragment */%}} One {{%/* /fragment */%}}
{{%/* fragment */%}} **Two** {{%/* /fragment */%}}
{{%/* fragment */%}} Three {{%/* /fragment */%}}
```

Press `Space` to play!

{{% fragment %}} One {{% /fragment %}}
{{% fragment %}} **Two** {{% /fragment %}}
{{% fragment %}} Three {{% /fragment %}}

---

A fragment can accept two optional parameters:

- `class`: use a custom style (requires definition in custom CSS)
- `weight`: sets the order in which a fragment appears

---

## Speaker Notes

Add speaker notes to your presentation

```markdown
{{%/* speaker_note */%}}
- Only the speaker can read these notes
- Press `S` key to view
{{%/* /speaker_note */%}}
```

Press the `S` key to view the speaker notes!

{{% speaker_note %}}
- Only the speaker can read these notes
- Press `S` key to view
{{% /speaker_note %}}

---

## Themes

- black: Black background, white text, blue links (default)
- white: White background, black text, blue links
- league: Gray background, white text, blue links
- beige: Beige background, dark text, brown links
- sky: Blue background, thin dark text, blue links

---

- night: Black background, thick white text, orange links
- serif: Cappuccino background, gray text, brown links
- simple: White background, black text, blue links
- solarized: Cream-colored background, dark green text, blue links

---

{{< slide background-image="/media/boards.jpg" >}}

## Custom Slide

Customize the slide style and background

```markdown
{{</* slide background-image="/media/boards.jpg" */>}}
{{</* slide background-color="#0000FF" */>}}
{{</* slide class="my-style" */>}}
```

---

## Custom CSS Example

Let's make headers navy colored.

Create `assets/css/reveal_custom.css` with:

```css
.reveal section h1,
.reveal section h2,
.reveal section h3 {
  color: navy;
}
```

---

# Questions?

[Ask](https://spectrum.chat/academic)

[Documentation](https://sourcethemes.com/academic/docs/managing-content/#create-slides)
