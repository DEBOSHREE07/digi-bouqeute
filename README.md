# A Bouquet for You

A little digital bouquet made of flowers, photos, music, and memories. This is a personal project, but it is also an invitation: **fork it, make it yours, and share what you create.**

## Make it your own

1. **Fork this project** on GitHub, then clone your fork or download it.
2. Open `index.html` in a browser. No build step is needed.
3. Add your own pictures and audio to the `images/` and `audio/` folders.
4. Edit the `CONFIG` object in `index.html` to change the names, flower memories, captions, photos, and letter.
5. Make it uniquely yours—change the colors, background, flowers, words, animations, or anything else you like.

### Add your photos

Put `.jpg`, `.jpeg`, or `.png` files in `images/`, then set the matching path on a flower in `CONFIG.flowers`:

```js
{
    title: "Our favorite day",
    text: "A little note about this memory.",
    image: "images/our-favorite-day.jpg"
}
```

Use a relative path and make sure the spelling and letter case match the file name. You can leave out `image` if you want a flower to open a text-only memory.

### Add your song

Put an `.mp3` file in `audio/` and update the audio source in `index.html`:

```html
<audio id="bgMusic" src="audio/your-song.mp3" loop preload="auto"></audio>
```

Browsers may wait for a visitor to tap the page before playing audio, so the music starts when the bouquet is opened.

### Change the background and colors

Replace `images/bg.jpg` with your own background image, or edit the `background-image` rule in the `body` styles in `index.html`. The main palette is set by CSS variables near the top of the `<style>` section, including `--bg`, `--bg2`, `--blush`, `--rose`, and `--gold`.

Want a **black** bouquet theme? Try a near-black `--bg` (such as `#080808`), then choose bright flower and accent colors so the bouquet still stands out. You can also change the flower colors in the JavaScript that draws the SVG flowers.

### Add more flowers and memories

Add or remove entries in `CONFIG.flowers`. Each entry becomes a flower you can open. Give every flower a title and a short note; add an `image` path when you want it to show a photo. The bouquet is drawn in the page's JavaScript, so you can also experiment with its shape, flower colors, petals, and animations.

## Share your creation

Make something sweet, silly, dramatic, cozy, or completely unexpected. Add a garden of flowers, a black-and-neon night sky, a playlist, a story, or a surprise of your own. **Use it, remix it, and make something unique—something yours.**

If you publish your remix, consider sharing a screenshot or link and telling others what you changed. Please only add photos, music, and other media that you have permission to share.

tag @eldestchildx on X


## License

This project is licensed under the MIT License.

```text
MIT License

Copyright (c) 2026 DEBOSHREE SINGHA

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

The license applies to this project's code and documentation, not automatically to photos, music, fonts, or other third-party assets. Make sure you have permission to use and redistribute those materials.
