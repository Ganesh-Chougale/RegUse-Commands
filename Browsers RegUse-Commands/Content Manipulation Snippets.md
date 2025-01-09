## **Content Manipulation Snippets**

1. **Enable Content Editing on the Page**  
   ```javascript
   document.body.contentEditable = true;
   ```

2. **Disable Content Editing on the Page**  
   ```javascript
   document.body.contentEditable = false;
   ```

3. **Change All Text on the Page**  
   Replace all text content on the page with custom text.  
   ```javascriptw
   document.body.innerText = "Hello, World!";
   ```

4. **Find and Replace Text on the Page**  
   Replace specific text on the page dynamically.  
   ```javascript
   document.body.innerHTML = document.body.innerHTML.replace(/OldText/g, "NewText");
   ```

5. **Clear All Text Content**  
   Remove all visible text on the page.  
   ```javascript
   document.body.innerText = "";
   ```

6. **Add Custom Text to the Page**  
   Append custom text to the end of the page content.  
   ```javascript
   document.body.innerHTML += "<p>Custom Text Added!</p>";
   ```

7. **Replace All Paragraphs with Custom Text**  
   ```javascript
   document.querySelectorAll('p').forEach(p => p.innerText = "Replaced Paragraph!");
   ```

8. **Change Page Title**  
   Update the page's title in the browser tab.  
   ```javascript
   document.title = "New Title";
   ```

9. **Remove All Elements of a Specific Type**  
   Example: Remove all `<div>` elements.  
   ```javascript
   document.querySelectorAll('div').forEach(div => div.remove());
   ```

10. **Highlight Specific Words on the Page**  
   Wrap specific words with a highlight (e.g., yellow background).  
   ```javascript
   document.body.innerHTML = document.body.innerHTML.replace(/HighlightThis/g, "<span style='background-color: yellow;'>HighlightThis</span>");
   ```

11. **Count All Words on the Page**  
   Calculate and log the total word count.  
   ```javascript
   console.log(document.body.innerText.split(/\s+/).length);
   ```

12. **Change All Headers (e.g., H1) to Custom Text**  
   ```javascript
   document.querySelectorAll('h1').forEach(h1 => h1.innerText = "Custom Header");
   ```

13. **Change Text Color on the Page**  
   Update all text to a specific color.  
   ```javascript
   document.body.style.color = "blue";
   ```

14. **Add a Watermark to the Page**  
   Inject a watermark text into the page background.  
   ```javascript
   document.body.style.backgroundImage = "url('data:image/svg+xml,<svg xmlns=\"http://www.w3.org/2000/svg\" viewBox=\"0 0 200 50\"><text x=\"0\" y=\"20\" fill=\"rgba(0,0,0,0.1)\" font-size=\"20\">Watermark</text></svg>')";
   ```

15. **Replace Text Based on User Input**  
   Prompt the user for a word to find and replace.  
   ```javascript
   const find = prompt("Enter the word to replace:");
   const replace = prompt("Enter the replacement word:");
   document.body.innerHTML = document.body.innerHTML.replace(new RegExp(find, "g"), replace);
   ```

16. **Add a Footer Message**  
   Append a footer message to the end of the page.  
   ```javascript
   const footer = document.createElement('div');
   footer.style.position = 'fixed';
   footer.style.bottom = '0';
   footer.style.width = '100%';
   footer.style.backgroundColor = 'black';
   footer.style.color = 'white';
   footer.style.textAlign = 'center';
   footer.innerText = "This is a footer message.";
   document.body.appendChild(footer);
   ```

17. **Reverse All Text on the Page**  
   Flip the text content backward.  
   ```javascript
   document.body.innerText = document.body.innerText.split('').reverse().join('');
   ```

18. **Wrap All Text in Quotes**  
   Enclose every word on the page in quotation marks.  
   ```javascript
   document.body.innerText = document.body.innerText.split(' ').map(word => `"${word}"`).join(' ');
   ```

19. **Replace Page Content with an ASCII Art**  
   ```javascript
   document.body.innerText = `
     ██████╗ ██████╗ ███████╗███╗   ██╗████████╗
     ██╔══██╗██╔══██╗██╔════╝████╗  ██║╚══██╔══╝
     ██████╔╝██████╔╝█████╗  ██╔██╗ ██║   ██║   
     ██╔═══╝ ██╔═══╝ ██╔══╝  ██║╚██╗██║   ██║   
     ██║     ██║     ███████╗██║ ╚████║   ██║   
     ╚═╝     ╚═╝     ╚══════╝╚═╝  ╚═══╝   ╚═╝   
   `;
   ```