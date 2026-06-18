# CS202 – Fundamentals of Front End Development
## Mid-Term Study Guide — Topics 01 to 72 (Easy English + Roman Urdu Hints)

This guide covers every topic from your handout, explained in simple English. Paper has 14 MCQs (14 marks) + 2 questions of 3 marks + 2 questions of 5 marks (16 marks), total 30 marks in 50 minutes. MCQs usually test **definitions and tags/properties**, so pay extra attention to bolded terms below.

---

## PART 1: Web Fundamentals (Topics 01–05)

### 01 – Front-End Development
Front-end (client-side) development means building the part of a website that the **user sees and interacts with directly** in the browser. The three front-end languages are **HTML** (structure), **CSS** (style), and **JavaScript** (behavior). A front-end developer is not a designer — they sit between the designer and the back-end developer, making sure content looks right and all user interactions work.
*Hint: Front-end = browser side; "design" alag chiz hai, front-end developer designer nahi hota.*

### 02 – URL (Uniform Resource Locator)
A **URL** is the global address of a resource on the web, and it's a type of **URI** (Uniform Resource Identifier — the general term for any web address/name). A URL has three parts: **protocol** (http/https/ftp), **resource location** (domain/IP), and an optional **resource name** (file). A **dynamic URL** contains special characters like `?`, `&`, `%`, `+`, `=` and carries parameters as key=value pairs. Since URLs can only use ASCII characters, **URL encoding** replaces unsafe characters with `%` plus hex digits, and replaces spaces with `+` or `%20`.
*Hint: URL ek address hai; agar usme ?, &, = ho to wo dynamic URL hai.*

### 03 – HTTP Basics
**HTTP** (HyperText Transfer Protocol) is the request-response protocol between a client (browser) and a server. The two main request methods are **GET** (requests data, limited length, can be cached) and **POST** (sends data to be processed, no length limit, never cached). **HTTPS** is the secure version of HTTP — all communication is encrypted and authenticated.
*Hint: GET = data lena (chota, cache hota hai); POST = data bhejna (bara, secure, cache nahi hota).*

### 04 – Web Server, Services and Agents
A **Web Server** is software that uses HTTP to deliver web pages to users on request. An **Application Server** provides both the tools to build web apps and the environment to run them. **Web Services** are client-server apps that communicate over the web (often using XML). A **Web/User Agent** is software (like a browser) that users use to talk to a web server.
*Hint: Browser = user agent; server jo files deta hai = web server.*

### 05 – Domain, Hosting, FTP
A **domain name** is the unique name of a website (e.g., google.com), mapped to an IP address through **DNS**. A domain has a **TLD** (Top Level Domain, e.g., .com), a **Second Level Domain** (must be unique, registered via ICANN), and optionally a **Sub Domain**. **Hosting** is a service that runs servers so your content stays available on the internet. **FTP** (File Transfer Protocol) transfers files between computers by splitting files into small packets and checking each one before sending the next.
*Hint: Domain = naam; Hosting = ghar jahan website rehti hai; FTP = files bhejnay ka tareeqa.*

---

## PART 2: HTML (Topics 06–27)

### 06/07 – HTML Introduction & Basics
**HTML** (HyperText Markup Language) is the standard language for creating web pages, read and displayed by browsers. Every HTML document starts with `<!DOCTYPE html>`, and the whole page sits between `<html>` and `</html>`, with visible content between `<body>` and `</body>`. Headings use `<h1>` to `<h6>`, paragraphs use `<p>`, and images use `<img>` with `src`, `alt`, `width`, and `height` attributes.
*Hint: DOCTYPE hamesha sabse upar; h1 sabse bara heading, h6 sabse chota.*

### 08 – Elements and Attributes
An **HTML element** has a start tag, content, and an end tag: `<tagname>content</tagname>`. Elements can be **nested** (one inside another) — the whole document is built of nested elements. Some elements have no content and are called **empty elements** (e.g., `<br>`). **Attributes** give extra information about an element, are written in the start tag, and come as name="value" pairs — common ones are `lang`, `title`, `href`, `src`, `alt`. Quotes (single or double) are used around attribute values.
*Hint: Attribute hamesha start tag mein hota hai, naam="value" ki shakal mein.*

### 09 – Heading and Paragraph
Headings (`<h1>`–`<h6>`) define document structure and are used by search engines to understand page content — they should never be used just to make text bold or big. `<hr>` draws a horizontal line to separate content. The `<head>` element holds metadata (not displayed), while `<title>` (shown in browser tab) and `<meta>` (charset, description, etc.) live inside `<head>`. `<br>` creates a line break without starting a new paragraph; browsers collapse extra spaces and blank lines into one.
*Hint: <head> ka heading se koi taluq nahi — head matlab meta-data (chupi hui info).*

### 10 – HTML Styling and Formatting
Every HTML element has a default style, which you can change using the `style` attribute (syntax: `style="property:value"`) — common properties: `color`, `font-family`, `font-size`, `text-align`, `background-color`. Formatting elements give text special meaning: `<b>` bold (no extra importance), `<strong>` bold with importance, `<i>` italic, `<em>` emphasized, `<small>`, `<mark>` (highlighted), `<del>` (deleted), `<sub>`/`<sup>` (subscript/superscript).
*Hint: <b> sirf bold dikhata hai, <strong> bold + ahmiyat (importance) dikhata hai.*

### 11 – HTML Quotations
`<q>` is for short quotations (browser adds quote marks automatically); `<blockquote>` is for long quotations (browser indents it). `<abbr>` marks an abbreviation, `<address>` marks contact info (usually shown italic), `<cite>` marks the title of a work (shown italic), and `<bdo>` overrides text direction (e.g., right-to-left).
*Hint: q = chota quote, blockquote = bara quote (indent hota hai).*

### 12 – HTML Computer Code
These tags keep fixed letter spacing for showing code: `<kbd>` for keyboard input, `<samp>` for sample computer output, `<code>` for programming code, and `<var>` for a mathematical variable.
*Hint: kbd=keyboard, samp=sample output, code=program code, var=variable.*

### 13 – HTML Comments
Comments use `<!-- comment text -->` and are not shown by the browser but help document the code or "comment out" lines while debugging. **Conditional comments** (e.g., `<!--[if IE 8]>`) target specific browsers.
*Hint: <!-- --> sirf developer ke liye, browser ignore karta hai.*

### 14 – HTML Links
Links use the `<a>` tag with the **href** attribute pointing to a destination (absolute URL like full address, or relative/local URL within the same site). The **target** attribute (`_blank`) opens a link in a new tab. Images can also act as links by wrapping `<img>` inside `<a>`. The **id** attribute creates bookmarks inside a page, linked using `#id`. Default link colors: unvisited = blue, visited = purple, active = red.
*Hint: href = kahan jana hai, target="_blank" = naya tab khulta hai.*

### 15 – HTML Images
Images use `<img src="url" alt="text">` — it's an empty tag (no closing tag needed). The **alt** attribute describes the image for screen readers (used by blind/visually impaired users) and shows if the image fails to load. Size can be set with `width`/`height` attributes or (recommended) the `style` attribute. Images can be stored locally, in a sub-folder, or on another server, and can float left/right of text using `style="float:left"`.
*Hint: alt attribute screen readers ke liye zaroori hai (jo log dekh nahi sakte unke liye).*

### 16 – HTML Tables (a & b)
Tables use `<table>`, rows use `<tr>`, data cells use `<td>`, and header cells use `<th>` (bold and centered by default). The `border` attribute adds a border; `border-collapse` in CSS merges double borders into one. `colspan` makes a cell span multiple columns, and `rowspan` makes it span multiple rows. `<caption>` adds a table title. A table can get a unique style by giving it an `id` and styling that id in CSS.
*Hint: colspan = column ko phailana, rowspan = row ko phailana.*

### 17 – HTML Lists
**Unordered lists** (`<ul>`) use bullets; list items use `<li>`. The bullet style is set with `list-style-type`: disc, circle, square, or none. **Ordered lists** (`<ol>`) use numbers/letters; the `type` attribute can be `1`, `A`, `a`, `I` (Roman upper), or `i` (Roman lower). **Description lists** use `<dl>` (list), `<dt>` (term), and `<dd>` (description). Lists can be displayed horizontally using CSS `display:inline` on `<li>`.
*Hint: ul = bullets, ol = numbers, dl/dt/dd = term aur uski description.*

### 18 – HTML Blocks
Most elements are either **block-level** (start/end with a new line, e.g., `<h1>`, `<p>`, `<table>`) or **inline** (no line break, e.g., `<b>`, `<a>`, `<img>`). `<div>` is a block-level container with no special meaning, used to group and style content. `<span>` is the inline equivalent, used to style a small part of text without breaking the line.
*Hint: div = block (naya line shuru), span = inline (line nahi tootti).*

### 19 – HTML Layout
Page layout is the structural arrangement of content. A common method uses several `<div>` elements (e.g., `id="header"`, `id="nav"`, `id="section"`, `id="footer"`) styled with CSS (`float`, `width`, `background-color`) to position each section. Tables can also be used for layout, though this is not their intended purpose.
*Hint: div + CSS = modern layout; table layout purana tareeqa hai.*

### 20 – HTML iFrame
`<iframe src="URL"></iframe>` embeds another HTML document inside the current page. `width` and `height` set its size; `style="border:none"` removes its default border. An iframe's `name` attribute can be used as a `target` for a link, so clicking a link loads content inside the iframe instead of the main page.
*Hint: iframe = ek webpage ke andar dusra webpage dikhana.*

### 21 – HTML Forms
The `<form>` element collects user input and contains form elements like `<input>` (text, radio, submit, etc.), grouped optionally with `<fieldset>` and `<legend>`. The **action** attribute defines where form data goes; **GET** is used for simple, non-sensitive data (visible in the URL), while **POST** is used for sensitive or large data (not visible in URL, more secure). Every input needs a **name** attribute to be submitted correctly.
*Hint: GET = URL mein dikhta hai (passive search); POST = chupi hui, sensitive data (password) ke liye.*

### 22 – HTML Colors
Colors combine Red, Green, and Blue light and can be specified three ways: **Hexadecimal** (`#RRGGBB`, e.g., `#FF0000` = red), **RGB** (`rgb(red,green,blue)`, values 0–255), or **color names** (140 standard names supported). RGB gives over 16 million possible colors (256×256×256).
*Hint: #FF0000 = red, #0000FF = blue — hex codes yaad rakhna useful hai.*

### 23 – HTML Head
The `<head>` element holds metadata: `<title>` (page title shown in tab/search results — required), `<style>` (internal CSS), `<link>` (connects external CSS file via `rel="stylesheet"`), `<meta>` (keywords, description, charset, author, refresh), `<script>` (JavaScript), and `<base>` (default URL/target for all relative links). In HTML5, `<html>`, `<head>`, and `<body>` tags can technically be omitted, but it's not good practice.
<br>
*Hint: <head> mein sab "invisible" info hoti hai — page par display nahi hoti.*

### 24 – HTML Entities and Symbols
Reserved characters like `<` and `>` are written using **character entities** so the browser doesn't confuse them with tags: `&lt;` for `<`, `&gt;` for `>`. A common one is `&nbsp;` (non-breaking space), since browsers normally collapse multiple spaces into one. Mathematical symbols and Greek letters also have entity names/numbers (e.g., `&euro;` for €).
*Hint: &lt; aur &gt; yaad rakho — yeh < aur > ke liye use hotay hain.*

### 25 – HTML Encoding (Character Sets)
**ASCII** was the first character set, supporting 127 characters (numbers, English letters, basic symbols). **ANSI** and **ISO-8859-1** extended this to 256 characters but were limited. **UTF-8** (Unicode) covers almost all characters/symbols in the world and is the default for HTML5, declared as `<meta charset="UTF-8">`.
*Hint: HTML5 ka default character set UTF-8 hai.*

### 26 – HTML URL Encoding
A URL follows the pattern `scheme://host.domain:port/path/filename`. Common schemes: **http** (normal, unencrypted), **https** (encrypted/secure), **ftp** (file transfer), **file** (local file). Since URLs only support ASCII, **URL encoding** converts other characters into `%` + hex digits, and spaces become `+` or `%20`.
*Hint: scheme://host.domain:port/path/filename — yeh structure yaad rakho.*

### 27 – HTML and XHTML
**XHTML** (EXtensible HyperText Markup Language) is HTML rewritten as strict XML. Key rules: the DOCTYPE is mandatory, elements must be properly nested and always closed (even empty ones, like `<br />`), all tags and attribute names must be lowercase, and all attribute values must be quoted. XHTML exists because "messy" HTML works in browsers but fails on stricter devices/parsers.
*Hint: XHTML = strict HTML — har tag close, lowercase, aur quotes zaroori.*

---

## PART 3: CSS (Topics 28–51)

### 28/29 – CSS Introduction
**CSS** (Cascading Style Sheets) describes how HTML elements should be displayed — separating content (HTML) from design (CSS). CSS syntax has a **selector** (the element to style) and a **declaration block** (`{property: value;}`) — e.g., `h1 { color: blue; font-size: 12px; }`. CSS comments are written as `/* comment */`.
*Hint: Selector { property: value; } — yeh basic CSS ka structure hai.*

### 30 – CSS Selectors
Important selectors: **`.class`** selects elements with that class (e.g., `.intro`); **`#id`** selects one element with that id; **`element`** selects all elements of that tag (e.g., `p`); **`element>element`** selects direct children (e.g., `div > p`); **`element1~element2`** selects siblings that come after; **`[attribute]`** and **`[attribute=value]`** select elements with that attribute.
*Hint: .class = dot se shuru, #id = hash se shuru.*

### 31 – CSS Insertion
CSS can be added three ways: **External** style sheet (a separate .css file linked via `<link rel="stylesheet" href="...">` in `<head>` — best for whole-site styling), **Internal** style sheet (`<style>` inside `<head>` — for one unique page), and **Inline** CSS (the `style` attribute on a single tag — for one unique element).
*Hint: External = sab pages, Internal = ek page, Inline = ek element.*

### 32 – CSS Background
**background-color** sets the background color of an element. **background-image** sets a background picture (repeats by default). **background-repeat** controls repeating (or shows it once), and **background-position** sets where the image appears. The shorthand property `background` combines all of these in one line.
*Hint: background-color = rang, background-image = tasveer, repeat = dohrana.*

### 33/34 – CSS Text and Fonts
**color** sets text color (hex, RGB, or name). **text-transform** changes case (uppercase/lowercase/capitalize); **text-indent** indents the first line. **font-family** sets the font, listing fallback fonts ending in a generic family (serif, sans-serif, monospace) — multi-word names need quotes (e.g., `"Times New Roman"`). **font-style** controls italic/oblique text. **font-size** can be set in pixels (fixed, full control) or **em** (relative — 1em = 16px by default, formula: pixels ÷ 16 = em), allowing users to resize text in the browser.
*Hint: px = fixed size, em = relative size (resize ho sakta hai).*

### 35 – CSS Links
Links can be styled like any element, plus they have four special states: **a:link** (unvisited), **a:visited** (visited), **a:hover** (mouse over), **a:active** (being clicked). `text-decoration: none` removes the underline, and `background-color` can be set per state.
*Hint: link → visited → hover → active — yeh order yaad rakho.*

### 36 – CSS Lists
The **list-style-type** property sets the bullet/number style (e.g., `circle`, `square`, `upper-roman`, `lower-alpha`). **list-style-image** uses a custom image as the bullet. The shorthand **list-style** combines type, position, and image in one declaration.
*Hint: list-style-type se bullet ka design badalta hai.*

### 37 – CSS Tables
**border** adds borders to table/th/td; **border-collapse: collapse** merges double borders into one. **width**/**height** set table size. **text-align** sets horizontal alignment (th is center by default, td is left by default); **vertical-align** sets vertical alignment. **padding** controls space inside cells.
*Hint: border-collapse: collapse — double lines ko ek line bana deta hai.*

### 38 – CSS Box Model
Every HTML element is treated as a box made of four parts (from inside out): **Content** (text/images), **Padding** (transparent space around content), **Border** (line around padding), and **Margin** (transparent space outside the border, clears area between elements). Understanding this is essential for setting an element's total width/height correctly.
*Hint: Content → Padding → Border → Margin (yehi order hai, andar se bahar tak).*

### 39 – CSS Border and Outline
**border-style** sets the type of border (solid, dotted, dashed, etc. — required for other border properties to work). **border-width** sets thickness; **border-color** sets color. Borders can be set per side (top/right/bottom/left), or all at once using the shorthand **border** property. An **outline** is similar to a border but drawn outside it and does NOT affect the element's total size.
*Hint: border-style pehle set karna zaroori hai, warna width/color kaam nahi karega.*

### 40 – CSS Margin and Padding
**Margin** is the transparent space outside the border (clears area around the element); **padding** is the space inside the border around the content (affected by background color). Both can be set per side (margin-top, etc.) or via shorthand with up to 4 values: `margin: top right bottom left;` (clockwise order).
*Hint: Margin = bahar ki khaali jaga, Padding = andar ki khaali jaga.*

### 41 – CSS Dimension
**width** and **height** properties control an element's size directly (e.g., for images). **min-height** sets a minimum height an element will always keep, even with little content.
*Hint: width/height = size, min-height = kam se kam itni height hogi.*

### 42 – CSS Align and Display
Block elements can be centered using `margin-left: auto; margin-right: auto;` with a set width. Elements can be aligned left/right using `position: absolute` or the simpler `float` property. The **display** property controls how an element appears: `display:none` hides it completely (removes its space), while `visibility:hidden` hides it but keeps its space. **Block** elements (h1, p, div) take full width with line breaks; **inline** elements (span, a) don't.
*Hint: display:none = jaga bhi gayab, visibility:hidden = sirf chupa, jaga rehti hai.*

### 43 – CSS Positioning, Floats & Combinators
Four positioning methods: **static** (default, normal flow), **fixed** (stays in place even when scrolling, relative to browser window), **relative** (positioned relative to its normal position, space still reserved), and **absolute** (positioned relative to nearest positioned ancestor, removed from normal flow). **z-index** controls stacking order when elements overlap. **float** pushes an element left/right, letting other content wrap around it; **clear** stops elements from wrapping. Four **combinators** join selectors: descendant (`div p`), child (`div > p`), adjacent sibling (`div + p`), and general sibling (`div ~ p`).
*Hint: static=normal, fixed=jama rehta hai, relative=apni jaga se hatke, absolute=parent ke hisab se.*

### 44 – CSS Pseudo-Class
A **pseudo-class** styles a special state of an element, written as `selector:pseudo-class`. Common ones: `a:link`, `a:visited`, `a:hover`, `a:active` for links, and `:first-child` (matches the first child element of its parent). The `:lang` pseudo-class sets rules for specific languages.
*Hint: pseudo-class = special "state" (jaise hover karte waqt).*

### 45 – CSS Pseudo-Element
A **pseudo-element** styles a specific part of an element, written with double colons: `selector::pseudo-element`. `::first-line` styles the first line of text; `::first-letter` styles the first letter; `::before` and `::after` insert content before/after an element's content; `::selection` styles text the user highlights/selects.
*Hint: pseudo-element = double colon (::) — element ka ek "hissa" style karta hai.*

### 46 – CSS Class
The **class selector** (`.classname`) applies a style to all elements with that class attribute. You can also restrict it to one tag type, e.g., `p.imp` only styles `<p>` elements with `class="imp"`. Class names can be alphanumeric but must not start with a number.
*Hint: Class number se start nahi ho sakta.*

### 47 – CSS Image Gallery
CSS can turn a group of images into a styled gallery by adding borders, padding, hover effects, and consistent sizing/spacing using simple selectors and the box model properties already covered.
*Hint: Image gallery = images ko CSS se design karna (border, padding, hover).*

### 48 – CSS Navigation Menu & Image Opacity
A navigation bar is built from a `<ul>`/`<li>` list, with `list-style-type:none` removing bullets and margin/padding set to 0. For a **vertical** nav bar, `<a>` elements get `display:block`. For a **horizontal** nav bar, `<li>` gets `display:inline` (simple method) or `float:left` (equal-width method). Separately, **opacity** creates transparent images (value 0.0 to 1.0, lower = more transparent), often combined with `:hover` for a fade effect.
*Hint: Horizontal menu = li{float:left} + a{display:block;width:..px}.*

### 49 – CSS Image Sprites
An **image sprite** combines several small images into one single image file, reducing server requests and saving bandwidth/loading time. CSS then shows only the needed part using `background-position` (e.g., `background: url(sprite.gif) -47px 0;`), and hover effects can swap to a second sprite image with hover states.
*Hint: Sprite = bohat si images ek hi file mein — loading time bachata hai.*

### 50 – CSS Media Types
Some CSS properties behave differently depending on the output device (screen vs. print). The **`@media`** rule lets you define different style rules for different media types in the same stylesheet (e.g., a different font size for print than for screen).
*Hint: @media rule se screen aur print ke liye alag style set hota hai.*

### 51 – CSS Attribute Selectors
These select elements based on their attributes: `[attribute]` (has the attribute), `[attribute=value]` (exact match), `[attribute~=value]` (contains the word in a space-separated list), `[attribute^=value]` (begins with), `[attribute$=value]` (ends with), `[attribute*=value]` (contains anywhere). Useful for styling forms without adding extra classes, e.g., `input[type="text"]`.
*Hint: ^ = shuru se match, $ = end se match, * = kahin bhi match.*

---

## PART 4: JavaScript (Topics 52–72)

### 52 – JavaScript Fundamentals
**JavaScript** is the programming language of the web — small, lightweight, and easy to learn. It can change HTML content (using `document.getElementById()`), change HTML attributes (e.g., swap an image's `src`), and change CSS styles dynamically, usually triggered by events like a button click.
*Hint: JS browser ke andar HTML/CSS ko "live" badalne ke liye hota hai.*

### 53 – JavaScript Syntax
JavaScript statements are separated by semicolons (`;`) and made up of **values** (literals — fixed numbers/strings — or variables), **operators** (`=`, `+`, `-`, etc.), **keywords** (like `var`), and **comments**. JavaScript is **case-sensitive** (`lastName` ≠ `lastname`) and commonly uses **camelCase** for naming variables (e.g., `firstName`).
*Hint: JS case-sensitive hai — capital/small letters ka farq parta hai.*

### 54 – JavaScript Statements
A statement tells the browser what to do, and statements execute one by one in order. Semicolons separate statements (multiple statements can be on one line if separated by `;`). JavaScript ignores extra white space, and statements can be grouped into **code blocks** using curly braces `{...}`.
*Hint: Statements hamesha order mein execute hotay hain — upar se neechay.*

### 55 – JavaScript Comments
**Single-line comments** start with `//` (rest of that line ignored). **Multi-line comments** start with `/*` and end with `*/`. Comments are used to explain code or to temporarily disable ("comment out") code while testing.
*Hint: // = ek line, /* */ = multiple lines.*

### 56 – JavaScript Variables and Operators (a & b)
Variables are containers for storing values, declared with the **var** keyword (e.g., `var x = 5;`). Variable names (**identifiers**) must start with a letter, `$`, or `_`, and are case-sensitive; reserved keywords cannot be used as names. The `=` sign is an **assignment** operator (not "equal to"). JavaScript has two basic data types here: **numbers** (no quotes) and **strings** (text in quotes). The `+` operator adds numbers but **concatenates** (joins) strings — and mixing a number with a string in `+` produces a string result (e.g., `"5" + 5` = `"55"`).
*Hint: "5" + 5 = "55" (text ban jata hai), lekin 5 + 5 = 10 (number rehta hai).*

### 57 – JavaScript Functions
A **function** is a reusable block of code that performs a task, defined as `function name(parameters) { code }`. It runs when "invoked" (called) — by an event, by code, or automatically. The **return** statement stops the function and sends a value back to where it was called. Functions let you reuse the same code with different arguments to get different results, and can be used like variables in expressions.
*Hint: Function = reusable code; return = function ka jawab wapas bhejta hai.*

### 58 – JavaScript Objects
**Objects** are containers for named values, called **properties**, and named actions, called **methods** (a method is simply a property that holds a function). Properties can hold primitive values, other objects, or even functions.
*Hint: Object ke andar properties (data) aur methods (functions) hotay hain.*

### 59 – JavaScript Scope
**Scope** defines where a variable can be accessed. **Local** variables (declared inside a function with `var`) can only be used inside that function and are deleted when it finishes. **Global** variables (declared outside any function) can be used by the entire page and exist until the page is closed. If you assign a value to an undeclared variable, it automatically becomes global.
*Hint: Local = ek function ke andar hi chalta hai; Global = sari page mein chalta hai.*

### 60 – JavaScript Events
**Events** are actions detected by the browser, such as a page loading, an input changing, or a button being clicked. Event handler attributes (like `onclick`) let you run JavaScript code when an event happens, e.g., `<button onclick="...">`. `this` inside an event handler refers to the element itself.
*Hint: onclick = button dabane par JS code chalana.*

### 61 – JavaScript Strings
A **string** stores text inside single or double quotes (e.g., `"Mike Slough"`). The built-in **length** property gives the number of characters. To use a quote character inside a matching-quote string, use the **escape character** (`\`), e.g., `'It\'s alright'`. Long lines can be broken after an operator, or by string addition (`+`), but not by a plain backslash in the middle of text.
*Hint: \' aur \" use karo jab quote ke andar wohi quote ana ho.*

### 62 – JavaScript Numbers
JavaScript has only one number type — always stored as **64-bit floating point**, with or without decimals, and supports scientific notation (`123e5`). Integers are accurate up to 15 digits; decimal math (e.g., `0.2 + 0.1`) can be slightly imprecise. `0xFF` is read as **hexadecimal**. Dividing by zero gives **Infinity**; an invalid math result gives **NaN** (Not a Number), checked using `isNaN()`.
*Hint: 0 se divide karo to Infinity milta hai; invalid math se NaN milta hai.*

### 63 – JavaScript Number Methods
Number methods return a new value without changing the original: **toString()** (number → string), **toFixed()** (rounds to a set number of decimals), **toPrecision()** (sets total digit length), **toExponential()** (exponential notation). Global functions **Number()**, **parseInt()** (returns a whole number), and **parseFloat()** (returns a decimal number) convert strings to numbers.
*Hint: parseInt = poora number nikalta hai, parseFloat = decimal ke saath nikalta hai.*

### 64 – JavaScript Math
The **Math** object provides mathematical tools: **Math.random()** (random number between 0 and 1), **Math.round()** (nearest whole number), **Math.ceil()** (rounds up), **Math.floor()** (rounds down), and **Math.min()/Math.max()** (lowest/highest of given values). It also provides constants like **Math.PI**.
*Hint: ceil = upar round, floor = neeche round, round = nearest round.*

### 65 – JavaScript Date
The **Date** object handles dates and times. `new Date()` creates the current date/time; you can also create dates from milliseconds, a date string, or specific year/month/day values. Common formats: **ISO** (YYYY-MM-DD, preferred), Long (e.g., "Mar 25 2015"), and Short (MM/DD/YYYY). **Get methods** (getDate, getDay, getFullYear, getHours, etc.) read parts of a date; **Set methods** (setDate, setFullYear, etc.) change parts of it. Dates can be compared directly using `<`, `>`, etc.
*Hint: ISO date format (YYYY-MM-DD) sabse standard/preferred hai.*

### 66 – More on Dates
`toString()`, `toUTCString()`, and `toDateString()` convert a date object into readable text formats. `Date.parse()` converts a valid date string into milliseconds since January 1, 1970 — useful for date math and comparisons.
*Hint: Date.parse() string ko milliseconds mein badalta hai.*

### 67 – JavaScript Arrays
An **array** stores multiple values in one variable, created with square brackets: `var cars = ["Toyota","Honda","BMW"];`. Elements are accessed by **index number**, starting at 0 (`cars[0]` = "Toyota"). Arrays are technically a special type of object — `typeof` returns "object" for them. The **length** property gives the number of elements; the easiest way to loop through an array is a `for` loop.
*Hint: Array index 0 se shuru hota hai, na ke 1 se.*

### 68 – JavaScript Arrays (Associative & Objects)
JavaScript does **not** support associative arrays (named indexes) — arrays always use numbered indexes; use **objects** instead when you need named (text) indexes. It's recommended to create arrays with `[]` rather than `new Array()`, since the latter can cause unexpected bugs.
*Hint: Named index chahiye to object use karo, number index chahiye to array.*

### 69 – Array Methods
Key array methods: **push()** (add to end), **pop()** (remove from end), **shift()** (remove from start), **splice()** (add/remove elements at any position), **sort()** (sorts alphabetically/numerically, can take a compare function), **reverse()** (reverses order), **concat()** (joins two arrays), and **slice()** (extracts part of an array into a new one without changing the original).
*Hint: push=end mein add, pop=end se remove, shift=start se remove.*

### 71 – JavaScript Comparisons
**Comparison operators**: `==` (equal value, ignores type), `===` (equal value AND type — strict), `!=`/`!==` (not equal), `>`, `<`, `>=`, `<=`. **Logical operators**: `&&` (and), `||` (or), `!` (not). The **ternary operator** gives a short if/else: `result = (condition) ? value1 : value2;`. Always prefer `===` for safe, predictable comparisons.
*Hint: == sirf value check karta hai, === value + type dono check karta hai (zyada safe).*

### 72 – JavaScript Conditions
**if** runs code only if a condition is true; **else** runs code if it's false; **else if** checks a new condition if the first was false; **switch** picks one of many code blocks based on a value. Syntax:
```javascript
if (condition) {
  // true case
} else if (condition2) {
  // second case
} else {
  // otherwise
}
```
*Hint: if=agar, else if=agar pehli baat false ho to ye check karo, else=warna.*

---

## Quick Revision Tips (for the exam)
For the 14 MCQs, focus on definitions, tag names, and "which property does what" — these are direct recall questions. For the 3-mark questions, expect short definitions or "write the syntax for X" type answers (e.g., write a `<table>` with colspan, or a CSS box model explanation). For the 5-mark questions, expect a slightly longer explanation with a small code example (e.g., explain CSS positioning methods with examples, or explain JavaScript functions with a sample function). Practice writing basic HTML/CSS/JS snippets by hand — that's usually the fastest way to lock in both the MCQ terms and the subjective answers.

Best of luck with your midterms!
