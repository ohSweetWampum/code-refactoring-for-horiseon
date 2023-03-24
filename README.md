# Horiseon Code Refactoring

## Technology Used

| Technology Used |                                              Resource URL                                              |
| --------------- | :----------------------------------------------------------------------------------------------------: |
| HTML            | [https://developer.mozilla.org/en-US/docs/Web/HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) |
| CSS             |  [https://developer.mozilla.org/en-US/docs/Web/CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)  |
| Git             |                              [https://git-scm.com/](https://git-scm.com/)                              |

## Description

[Visit the Deployed Site](https://ohsweetwampum.github.io/code-refactoring-for-horiseon/)

Code refactoring is the process of restructuring exsisting code to improve it's structure in a way that does not change it's original functionality. Horiseon wanted their code to be more accessible and consolidated, but did not want the webpage behavior to change, so it was decided that I should refactor it.

This refactoring was done by:

- Changing all non-semantic html elements into semantic elements.
- Including an alt attribute in all the image elements
- Fixing a broken link
- Getting rid of redundant CSS class selectors (combined multiple class selectors into 1 class selector)
- Getting rid of id selctors that were uneccessary

## Example of the html Code Refactoring

```html
<header>
  <h1>Hori<span class="seo">seo</span>n</h1>
  <!-- replcaed <div> elements with <nav> elements as this is actually describes the purpose of this <ul>. <nav> is semantic. -->
  <nav>
    <ul>
      <li>
        <a href="#search-engine-optimization">Search Engine Optimization</a>
      </li>
      <li>
        <a href="#online-reputation-management">Online Reputation Management</a>
      </li>
      <li>
        <a href="#social-media-marketing">Social Media Marketing</a>
      </li>
    </ul>
  </nav>
</header>
<!-- changed the <div> element to a <figure> element as it better describes the actual layout of the webpage and is a semantic element-->
<figure class="hero"></figure>
```

As you can see I introduced semantic elements to the code such as; `html<header>, <nav>, and <figure> `

## Example of CSS Code Refactoring

```css
/*  deleted all the 3 different class selctors (benefit-lead, benefit-brand, benefit-cost) and combined them into one selector and called it "aside-properties" as all three old selectors had the same properties. This is a huge time and space saver */
.aside-properties h3 {
  margin-bottom: 10px;
  text-align: center;
}
```

## Usage

The website has a navigation bar which your can use to jump to the topic your are interested in.

![image](/assets/images/Screenshot%202023-03-23%20at%208.54.14%20PM.png)

Depending on what topic you selcted, you will be directed to one of these three section where you can read more about the topic. An aside section describes more benefits of using Horiseon's services.

![alt text](/assets/images/Screenshot%202023-03-23%20at%208.54.26%20PM.png)

## Learning Points

Main things I learned were:

- How to consolidate CSS selectors
- How to structure html code properly using semantic elements

## Author Info

Matthew Gibson

- [Portfolio](https://github.com/ohSweetWampum)
- [LinkedIn](https://www.linkedin.com/in/matthew-gibson-6b9b12237/)
- [Github](https://github.com/ohSweetWampum)

## Credits

[w3schools.com](https://www.w3schools.com/css/css_selectors.asp)

[w3schools.com](https://www.w3schools.com/html/html5_semantic_elements.asp)

## License

MIT License

Copyright (c) [2023] [ohSweetWampum]

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

---
