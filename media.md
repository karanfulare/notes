## 1. `<img>`: Embeds images.

- Example: `<img src="image.jpg" alt="Description">`

## `<img>` Tag

The `<img>` tag is used to embed images in an HTML document.

### Attributes

1. `src` (required): Specifies the source URL of the image.

   - **Example**: `<img src="image.jpg" alt="Description">`

2. `alt` (optional): Provides alternative text for the image, useful for screen readers and when the image cannot be displayed.

   - **Example**: `<img src="image.jpg" alt="A beautiful sunset">`

3. `width` (optional): Sets the width of the image in pixels.

   - **Example**: `<img src="image.jpg" alt="Description" width="300">`

4. `height` (optional): Sets the height of the image in pixels.

   - **Example**: `<img src="image.jpg" alt="Description" height="200">`

5. `title` (optional): Adds a tooltip that appears when the user hovers over the image.

   - **Example**: `<img src="image.jpg" alt="Description" title="Image tooltip">`

6. `loading` (optional): Specifies how the browser should load the image. Values can be `"auto"`, `"eager"`, or `"lazy"`.

   - `"auto"`: Default behavior, loads the image immediately.
   - `"eager"`: Loads the image as soon as possible.
   - `"lazy"`: Defers loading until it's in the viewport (lazy loading).
   - **Example**: `<img src="image.jpg" alt="Description" loading="lazy">`

7. `decoding` (optional): Indicates how the image should be decoded. Values can be `"auto"`, `"sync"`, or `"async"`.

   - `"auto"`: Default behavior, allows the browser to choose.
   - `"sync"`: Decodes the image synchronously.
   - `"async"`: Decodes the image asynchronously.
   - **Example**: `<img src="image.jpg" alt="Description" decoding="async">`

8. `sizes` (optional): Suggests the browser image display size based on layout breakpoints.

   - **Example**: `<img srcset="image.jpg 300w, image-large.jpg 600w" sizes="(max-width: 600px) 300px, 600px">`

9. `srcset` (optional): Provides multiple sources and sizes for the image to be used in responsive design.
   - **Example**: `<img srcset="image.jpg 300w, image-large.jpg 600w" sizes="(max-width: 600px) 300px, 600px">`

### Defaults

- If the `alt` attribute is missing, some browsers display the image's filename as a fallback.
- If the `width` and `height` attributes are missing, the image's natural dimensions are used.

### Exceptions

- The `src` attribute is required. Without it, the image won't load.
- If the `alt` attribute is omitted or empty, it may result in accessibility issues and is considered bad practice.
- Providing both `width` and `height` attributes is recommended to avoid layout shifts as the image loads.
- Using `loading="lazy"` or `loading="eager"` is a good practice for optimizing page loading.

Remember to always provide alternative text (`alt`) for images, as it improves accessibility and ensures that the content remains understandable even when images fail to load.

## 2. `<audio>`: Embeds audio content.

- Example: `<audio src="music.mp3" controls></audio>`

## `<audio>` Tag

The `<audio>` tag is used to embed audio content in an HTML document.

### Attributes

1. `src` (required): Specifies the source URL of the audio file.

   - **Example**: `<audio src="audio.mp3" controls></audio>`

2. `controls` (optional): Adds audio controls like play, pause, and volume to the player.

   - **Example**: `<audio src="audio.mp3" controls></audio>`

3. `autoplay` (optional): Automatically starts playing the audio when the page loads.

   - **Example**: `<audio src="audio.mp3" autoplay></audio>`

4. `loop` (optional): Causes the audio to start over again when it reaches the end.

   - **Example**: `<audio src="audio.mp3" controls loop></audio>`

5. `preload` (optional): Hints how much buffering the browser should do before starting to play. Values can be `"auto"`, `"metadata"`, or `"none"`.

   - `"auto"`: Default behavior, the browser decides how much to buffer.
   - `"metadata"`: Buffer only the metadata (e.g., duration) of the audio.
   - `"none"`: No buffering; the audio is loaded only when requested.
   - **Example**: `<audio src="audio.mp3" preload="auto"></audio>`

6. `muted` (optional): Mutes the audio by default. Users can unmute it using the controls.

   - **Example**: `<audio src="audio.mp3" controls muted></audio>`

7. `volume` (optional): Sets the initial volume level. Values range from `0.0` (silent) to `1.0` (maximum volume).
   - **Example**: `<audio src="audio.mp3" controls volume="0.5"></audio>`

### Defaults

- If the `controls` attribute is missing, the audio will play without user controls.
- If `autoplay` is omitted, the audio won't start automatically.
- Without `loop`, the audio will play once and stop.
- Browsers typically preload audio content to optimize playback.

### Exceptions

- The `src` attribute is required. Without it, the audio won't load.
- Autoplaying audio can be intrusive, so it should be used sparingly and with consideration for the user experience.
- Not all audio formats are supported by all browsers, so it's essential to provide alternative formats (e.g., MP3 and OGG) using the `<source>` element within the `<audio>` tag for broader compatibility.

Remember to use the `<source>` element within the `<audio>` tag to provide multiple audio formats to ensure compatibility across different browsers:

```html
<audio controls>
  <source src="audio.mp3" type="audio/mpeg" />
  <source src="audio.ogg" type="audio/ogg" />
  Your browser does not support the audio element.
</audio>
```

## 3. `<video>`: Embeds video content.

- Example: `<video src="video.mp4" controls></video>`

- ## `<video>` Tag

  The `<video>` tag is used to embed video content in an HTML document.

  ### Attributes

  1. `src` (required): Specifies the source URL of the video file.

- **Example**: `<video src="video.mp4" controls></video>`

  2. `controls` (optional): Adds video controls like play, pause, and volume to the player.

- **Example**: `<video src="video.mp4" controls></video>`

  3. `autoplay` (optional): Automatically starts playing the video when the page loads.

- **Example**: `<video src="video.mp4" autoplay></video>`

  4. `loop` (optional): Causes the video to start over again when it reaches the end.

- **Example**: `<video src="video.mp4" controls loop></video>`

  5. `preload` (optional): Hints how much buffering the browser should do before starting to play. Values can be `"auto"`, `"metadata"`, or `"none"`.

- `"auto"`: Default behavior, the browser decides how much to buffer.
- `"metadata"`: Buffer only the metadata (e.g., duration) of the video.
- `"none"`: No buffering; the video is loaded only when requested.
- **Example**: `<video src="video.mp4" preload="auto"></video>`

  6. `muted` (optional): Mutes the video by default. Users can unmute it using the controls.

- **Example**: `<video src="video.mp4" controls muted></video>`

  7. `width` (optional): Sets the width of the video player.

- **Example**: `<video src="video.mp4" width="320" height="240" controls></video>`

  8. `height` (optional): Sets the height of the video player.

- **Example**: `<video src="video.mp4" width="320" height="240" controls></video>`

  ### Defaults

  - If the `controls` attribute is missing, the video will play without user controls.
  - If `autoplay` is omitted, the video won't start automatically.
  - Without `loop`, the video will play once and stop.
  - Browsers typically preload video content to optimize playback.

  ### Exceptions

  - The `src` attribute is required. Without it, the video won't load.
  - Autoplaying videos can be intrusive, so they should be used sparingly and with consideration for the user experience.
  - Not all video formats are supported by all browsers, so it's essential to provide alternative formats (e.g., MP4, WebM, and OGG) using the `<source>` element within the `<video>` tag for broader compatibility.

  Remember to use the `<source>` element within the `<video>` tag to provide multiple video formats to ensure compatibility across different browsers:

  ```html
  <video controls>
    <source src="video.mp4" type="video/mp4" />
    <source src="video.webm" type="video/webm" />
    <source src="video.ogv" type="video/ogg" />
    Your browser does not support the video element.
  </video>
  ```

## 4. `<iframe>`: Embeds external web content (e.g., YouTube videos).

- **Example**

```html
<iframe src="https://www.youtube.com/embed/VIDEO_ID" frameborder="0" allowfullscreen></iframe>
```

## 5. `<figure>`: Groups media content with a caption.

- **Example**
  ```html
  <figure>
    <img src="image.jpg" alt="Description" />
    <figcaption>Caption for the image.</figcaption>
  </figure>
  ```

## 6. `<figcaption>`: Provides a caption for a `<figure>` element.

- **Example**

```html
<figcaption>Caption for the media content.</figcaption>
```

## 7. `<audio>` and `<source>`: Allows specifying multiple audio sources for compatibility.

- **Example**

```html
<audio controls>
  <source src="music.mp3" type="audio/mpeg" />
  <source src="music.ogg" type="audio/ogg" />
  Your browser does not support the audio element.
</audio>
```

## 8. `<video>` and `<source>`: Allows specifying multiple video sources for compatibility.

- **Example**
  ```html
  <video controls>
    <source src="video.mp4" type="video/mp4" />
    <source src="video.webm" type="video/webm" />
    Your browser does not support the video element.
  </video>
  ```

## 9. `<track>`: Provides text tracks for video or audio elements.

- **Example**
  ```html
  <video controls>
    <source src="video.mp4" type="video/mp4" />
    <track label="English" kind="subtitles" src="subtitles_en.vtt" srclang="en" />
    <track label="Spanish" kind="subtitles" src="subtitles_es.vtt" srclang="es" />
    Your browser does not support the video element.
  </video>
  ```

## 10. `<canvas>`: Used for drawing graphics using JavaScript.

- **Example**

```html
<canvas id="myCanvas" width="200" height="100"></canvas>
```

## 11. `<svg>`: Embeds scalable vector graphics.

- **Example**

```html
<svg width="100" height="100"><circle cx="50" cy="50" r="40" stroke="black" stroke-width="2" fill="red" /></svg>
```

## 12. `<embed>`: Embeds external content (e.g., Flash).

- **Example**

```html
<embed src="flash.swf" type="application/x-shockwave-flash" />
```

## 13. `<object>`: Embeds external content and multimedia objects.

- **Example**

```html
<object data="file.pdf" type="application/pdf" width="500" height="400"></object>
```

## 14. `<param>`: Defines parameters for an `<object>` element.

- **Example**

  ```html
  <param name="autoplay" value="true" />
  ```

## 15. `<source>`: Specifies alternative media resources for `<picture>` and `<video>` elements.

- **Example**
  ```html
  <picture>
    <source srcset="image.webp" type="image/webp" />
    <img src="image.jpg" alt="Description" />
  </picture>
  ```

These are examples of various HTML media tags and their usage. When working with these tags, you can adjust attributes like `src`, `alt`, `controls`, `width`, and `height` to suit your specific media content and requirements.
