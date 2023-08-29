1. `<img>`: Embeds images.

   - Example: `<img src="image.jpg" alt="Description">`

2. `<audio>`: Embeds audio content.

   - Example: `<audio src="music.mp3" controls></audio>`

3. `<video>`: Embeds video content.

   - Example: `<video src="video.mp4" controls></video>`

4. `<iframe>`: Embeds external web content (e.g., YouTube videos).

   - Example: `<iframe src="https://www.youtube.com/embed/VIDEO_ID" frameborder="0" allowfullscreen></iframe>`

5. `<figure>`: Groups media content with a caption.

   - Example:
     ```markdown
     <figure>
       <img src="image.jpg" alt="Description">
       <figcaption>Caption for the image.</figcaption>
     </figure>
     ```

6. `<figcaption>`: Provides a caption for a `<figure>` element.

   - Example: `<figcaption>Caption for the media content.</figcaption>`

7. `<audio>` and `<source>`: Allows specifying multiple audio sources for compatibility.

   - Example:
     ```markdown
     <audio controls>
       <source src="music.mp3" type="audio/mpeg">
       <source src="music.ogg" type="audio/ogg">
       Your browser does not support the audio element.
     </audio>
     ```

8. `<video>` and `<source>`: Allows specifying multiple video sources for compatibility.

   - Example:
     ```markdown
     <video controls>
       <source src="video.mp4" type="video/mp4">
       <source src="video.webm" type="video/webm">
       Your browser does not support the video element.
     </video>
     ```

9. `<track>`: Provides text tracks for video or audio elements.

   - Example:
     ```markdown
     <video controls>
       <source src="video.mp4" type="video/mp4">
       <track label="English" kind="subtitles" src="subtitles_en.vtt" srclang="en">
       <track label="Spanish" kind="subtitles" src="subtitles_es.vtt" srclang="es">
       Your browser does not support the video element.
     </video>
     ```

10. `<canvas>`: Used for drawing graphics using JavaScript.

    - Example: `<canvas id="myCanvas" width="200" height="100"></canvas>`

11. `<svg>`: Embeds scalable vector graphics.

    - Example: `<svg width="100" height="100"><circle cx="50" cy="50" r="40" stroke="black" stroke-width="2" fill="red" /></svg>`

12. `<embed>`: Embeds external content (e.g., Flash).

    - Example: `<embed src="flash.swf" type="application/x-shockwave-flash">`

13. `<object>`: Embeds external content and multimedia objects.

    - Example: `<object data="file.pdf" type="application/pdf" width="500" height="400"></object>`

14. `<param>`: Defines parameters for an `<object>` element.

    - Example: `<param name="autoplay" value="true">`

15. `<source>`: Specifies alternative media resources for `<picture>` and `<video>` elements.
    - Example:
      ```markdown
      <picture>
        <source srcset="image.webp" type="image/webp">
        <img src="image.jpg" alt="Description">
      </picture>
      ```

These are examples of various HTML media tags and their usage. When working with these tags, you can adjust attributes like `src`, `alt`, `controls`, `width`, and `height` to suit your specific media content and requirements.
