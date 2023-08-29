1. `href` (Hypertext Reference):

   - Description: Specifies the URL of the linked resource, which can be a web page, an image, a file, or another webpage.
   - Example: `<a href="https://www.example.com">Visit Example</a>`

2. `target`:

   - Description: Specifies where the linked resource should be displayed. Common values include `_blank` (in a new tab or window), `_self` (in the same frame or window), `_parent` (in the parent frame), and `_top` (in the full body of the window).
   - Example: `<a href="https://www.example.com" target="_blank">Visit Example in a new tab</a>`

3. `download`:

   - Description: Suggests that the target resource should be downloaded by the browser rather than navigated to. It specifies the filename for the downloaded file.
   - Example: `<a href="document.pdf" download="my-document.pdf">Download PDF</a>`

4. `rel` (Relationship):

   - Description: Specifies the relationship between the current document and the linked resource. Common values include `nofollow` (to indicate that search engines should not follow the link) and `noopener` (to protect against security vulnerabilities).
   - Example: `<a href="https://www.example.com" rel="noopener">Visit Example</a>`

5. `title`:

   - Description: Provides additional information about the linked resource that is displayed as a tooltip when the user hovers over the link.
   - Example: `<a href="https://www.example.com" title="Visit Example">Example</a>`

6. `id`:

   - Description: Specifies a unique identifier for the hyperlink. It is often used in conjunction with JavaScript to manipulate or reference the link.
   - Example: `<a href="#section-1" id="link-1">Jump to Section 1</a>`

7. `class`:

   - Description: Assigns one or more CSS classes to the hyperlink, allowing for custom styling and targeting through CSS.
   - Example: `<a href="https://www.example.com" class="btn btn-primary">Visit Example</a>`

8. `style`:

   - Description: Specifies inline CSS styles to apply to the hyperlink, enabling custom styling directly in the HTML.
   - Example: `<a href="https://www.example.com" style="color: blue; text-decoration: underline;">Visit Example</a>`

9. `aria-*` (Accessible Rich Internet Applications):

   - Description: Attributes that improve web accessibility by providing additional information to screen readers and assistive technologies.
   - Example: `<a href="https://www.example.com" aria-label="Visit Example">Example</a>`

10. `data-*` (Custom Data Attributes):
    - Description: Custom attributes that allow you to store extra information with the hyperlink. These attributes are often used for JavaScript interactions.
    - Example: `<a href="#" data-action="open-modal">Open Modal</a>`
