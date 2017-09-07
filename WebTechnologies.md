## Web Technologies [link](https://developer.mozilla.org/en-US/docs/Web)
### Basics
#### HTML
- Hyper text markup language, describes and defines content of a webpage.
- Annotations to mark how a particular piece of content should be displayed.
- Elements applied to text provides different meaning and structure and embed media
- \<meta charset="UTF-8"><meta
- HTML entities => < > " ' &  => \&lt; \&gt; \&quot; \&apos; \&amp;
- img, video are replaced elements. Contents determined by external resource
  - img => alt texts are read by screen readers
  - Text only browsers like lynx use alt text to describe image
  - img has width and height attributes
  - \<figure> and \<figcaption> to semantically add captions to images
  - Screen Readers and assistive technology 
- Video
  - different codecs are supported by different browsers => codecs used to make files manageable
  - Video uses container formats like WebM (firefox, chrom), MP4 (IE, safari) etc
  
```html
  <video controls>
    <source src="rabbit320.mp4" type="video/mp4">
    <source src="rabbit320.webm" type="video/webm">
    <p>Your browser doesn't support HTML5 video. Here is a <a href="rabbit320.mp4">link to the video</a> instead.</p>
  </video>
```  
  - In this case the browser will go through the <source> elements and play the first one that it has the codec to support.
  - Video tag supports: src, controls, loop, poster, autoplay, muted etc
  - Audio tag supports all above except poster, width and height
  - WebVTT, text file with time to show the text, used for subtitles, captions, descriptions
    - To make it work, save as .vtt files
    - link to the file using <track> element takes, src, kind (subtitles | captions | descriptions), srclang
  - href vs src :
    - href is hypertext reference; used for referencing to external documents
    - src is used in replaced elements; parsing is paused till the file is obtained
    - with HTML5 , there are additional attributes for loading and executing scripts
      - async : script executed asynchronously, as soon as it is available
      - defer: executed when the page has finished parsing
      - else, script fetched and executed immediately before user agent continues parsing the page
  - Use \<em> and \<strong> over \<i> and \<b>; semantic elements vs purely presentational elements
  - Links \<a> are what makes web a web. use relative hrefs for local pages otherwise extra DNS lookup by absolute URLs
  - ˚˚ download attribute in anchor tag used for default save filename
  - URL encoded href for emails mailto:nowhere@mozilla.org?cc=nobody@mozilla.org&subject=This%20is%20the%20subject
