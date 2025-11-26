---
{"dg-publish":true,"permalink":"/how-to-use-obsidian/"}
---

ty
> asd

asd

| **Feature**              | **Syntax**                                                              | **Example**                                  |
| ------------------------ | ----------------------------------------------------------------------- | -------------------------------------------- |
| **Basic Callout**        | `> [!NOTE] Title`                                                       | > [!NOTE] Here is a Note                     |
| **Foldable (Collapsed)** | `> [!TIP]- Collapsed Tip`                                               | > [!TIP]- This Tip is Hidden                 |
| **Custom Title**         | `> [!INFO] Important Information`                                       | > [!INFO] Important Information              |
| **Nested Callout**       | `> [!FAQ] Main Question`<br><br>  <br><br>`> > [!ANSWER] Nested Answer` | You must use an extra `>` for nested blocks. |

> [!Note] AS

> [!TIP]- Collapsed Tip

> [!INFO] Important Information

> [!FAQ] Main Question
> > [!ANSWER] Nested Answer


| **Feature**        | **Syntax**           | **Example**          | **Notes**                           |
| ------------------ | -------------------- | -------------------- | ----------------------------------- |
| **Unordered List** | `- item` or `* item` | `- Milk`             | Use `Tab` to create nested lists.   |
| **Ordered List**   | `1. item`            | `1. First Step`      | The numbers update automatically.   |
| **Task List**      | `- [ ] task text`    | `- [ ] Finish Draft` | Click the box to toggle completion. |
| **Completed Task** | `- [x] task text`    | `- [x] Send Email`   | Completed item.                     |

- item 1
- item 2

1. item 1
2. item 2

- [ ] A
- [ ] B
- [ ] C


- [x] A
- [x] B
- [x] C

| **Feature**         | **Syntax**                    | **Example**                    | **Notes**                                     |
| ------------------- | ----------------------------- | ------------------------------ | --------------------------------------------- |
| **Wikilink**        | `[[Note Name]]`               | `[[Project Plan]]`             | Links to another note in your vault.          |
| **Link with Alias** | `[[Note Name\|Display Text]]` | `[[Project Plan\|Go to Plan]]` | Changes the text that is displayed.           |
| **Internal Embed**  | `![[File Name.ext]]`          | `![[my-chart.png]]`            | Embeds the content (Image, PDF, Video).       |
| **Resize Image**    | `![[Image.png\|300]]`         | `![[my-chart.png\|300]]`       | Sets the display **width** to 300px.          |
| **Block Reference** | `[[Note Name#^block-id]]`     | `[[Summary#^idea]]`            | Links directly to a specific paragraph/block. |
| **External Link**   | `[Link Text](URL)`            | `[Google](https://google.com)` | Standard Markdown link to the web.            |
Alrighty

|**Feature**|**Syntax**|**Example**|**Result**|
|---|---|---|---|
|**Headings**|`# Heading 1`|`# My Project`|Large Title|
||`## Heading 2`|`## Key Concepts`|Sub-section|
||`### Heading 3`|`### Details`|Deeper level|
|**Bold**|`**text**` or `__text__`|`**Important**`|**Important**|
|**Italic**|`*text*` or `_text_`|`*note*`|_note_|
|**Bold & Italic**|`***text***`|`***Urgent***`|**_Urgent_**|
|**Strikethrough**|`~~text~~`|`~~mistake~~`|~~mistake~~|
|**Highlight**|`==text==`|`==Key Idea==`|$\text{Highlight}$ (Requires Obsidian's extension)|
|**Horizontal Rule**|`---` or `***`|`---`|A dividing line|
|**Blockquote**|`> text`|`> "A wise man speaks"`|> "A wise man speaks"|
asd

| **Feature**      | **Syntax**                                               | **Example**                                                                   | **Notes**                                                             |
| ---------------- | -------------------------------------------------------- | ----------------------------------------------------------------------------- | --------------------------------------------------------------------- |
| **Inline Code**  | `` `code` ``                                             | `The variable is` `x`                                                         | Used for single words or short phrases of code/variables.             |
| **Code Block**   | `\text{`javascript}``<br> `// code here` <br>``\text{`}` | `css\nbody { background: #fff; }`                                             | The first line tells Obsidian which language to use for highlighting. |
| **Inline Math**  | `$E=mc^2$`                                               | The formula is $E=mc^2$                                                       | Uses LaTeX syntax for mathematical expressions.                       |
| **Display Math** | `$$\frac{\partial^2 u}{\partial t^2}$$`                  | $$\frac{\partial^2 u}{\partial t^2} = c^2 \frac{\partial^2 u}{\partial x^2}$$ | Centers the equation on its own line.                                 |


| Header 1  | Header 2  | Header 3  |
| --------- | --------- | --------- |
| Content A | Content B | Content C |
| More A    | More B    | More C    |
Alignment (Using colons `:` in the separator line)
IN TABLES

| **Syntax** | **Description** |
| ---------- | --------------- |
| `:--`      | Left-aligned    |
| `:--:`     | Center-aligned  |
| `--:`      | Right-aligned   |


|**HTML Element**|**Use Case**|**Example**|
|---|---|---|
|`<br>`|**Forced Line Break**|Use to start a new line _without_ starting a new paragraph.|
|`<u>`|**Underline**|`<u>Underline Text</u>`|
|`<center>` (or CSS)|**Center Text/Images**|`<h1><center>Title</center></h1>`|


<p align='center'>
<span style="font-size: 1.5em;"> Centered Big font </span>
</p>



