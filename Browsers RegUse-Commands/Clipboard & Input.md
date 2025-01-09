## **Clipboard & Input**:

1. **Copy Text to Clipboard**
   ```javascript
   function copyTextToClipboard(text) {
     const textArea = document.createElement('textarea');
     textArea.value = text;
     document.body.appendChild(textArea);
     textArea.select();
     document.execCommand('copy');
     document.body.removeChild(textArea);
   }

   copyTextToClipboard('Text to copy');
   ```

2. **Paste Clipboard Content into Input Field**
   ```javascript
   document.querySelector('input').addEventListener('click', () => {
     navigator.clipboard.readText().then(text => {
       document.querySelector('input').value = text;
     });
   });
   ```

3. **Select All Text in Input Field**
   ```javascript
   document.querySelector('input').select();
   ```

4. **Clear Text Input Field**
   ```javascript
   document.querySelector('input').value = '';
   ```

5. **Disable Text Input**
   ```javascript
   document.querySelector('input').disabled = true;
   ```

6. **Enable Text Input**
   ```javascript
   document.querySelector('input').disabled = false;
   ```

7. **Set Placeholder Text**
   ```javascript
   document.querySelector('input').placeholder = 'Enter your name';
   ```

8. **Auto-Fill Text Input with Random Text**
   ```javascript
   document.querySelector('input').value = Math.random().toString(36).substring(7);
   ```

9. **Auto-Select Text Inside Input Field**
   ```javascript
   document.querySelector('input').setSelectionRange(0, document.querySelector('input').value.length);
   ```

10. **Track Text Input Changes**
    ```javascript
    document.querySelector('input').addEventListener('input', (event) => {
      console.log('Input changed:', event.target.value);
    });
    ```

11. **Trigger Input Event Programmatically**
    ```javascript
    document.querySelector('input').dispatchEvent(new Event('input'));
    ```

12. **Limit Input to Certain Characters (e.g., Numbers)**
    ```javascript
    document.querySelector('input').addEventListener('input', function() {
      this.value = this.value.replace(/[^0-9]/g, '');
    });
    ```

13. **Auto Focus on an Input Field**
    ```javascript
    document.querySelector('input').focus();
    ```

14. **Select Text Content from a Textarea**
    ```javascript
    document.querySelector('textarea').select();
    ```

15. **Auto Resize Textarea Based on Content**
    ```javascript
    const textarea = document.querySelector('textarea');
    textarea.addEventListener('input', function () {
      this.style.height = 'auto';
      this.style.height = (this.scrollHeight) + 'px';
    });
    ```

16. **Get User Input and Display in an Alert**
    ```javascript
    const userInput = prompt('Please enter something:');
    alert('You entered: ' + userInput);
    ```

17. **Prevent Default Input Action**
    ```javascript
    document.querySelector('input').addEventListener('keydown', (event) => {
      event.preventDefault(); // Prevents any key input
    });
    ```

18. **Paste Clipboard Content into Textarea**
    ```javascript
    document.querySelector('textarea').addEventListener('focus', () => {
      navigator.clipboard.readText().then(text => {
        document.querySelector('textarea').value = text;
      });
    });
    ```

19. **Prevent Form Submission**
    ```javascript
    document.querySelector('form').addEventListener('submit', (event) => {
      event.preventDefault(); // Prevent form submission
    });
    ```

20. **Trigger Paste Action Programmatically**
    ```javascript
    const pasteEvent = new ClipboardEvent('paste', {
      dataType: 'text/plain',
      data: 'Some pasted content'
    });
    document.querySelector('input').dispatchEvent(pasteEvent);
    ```

21. **Track Clipboard Copy Action**
    ```javascript
    document.addEventListener('copy', (event) => {
      console.log('Content copied to clipboard:', event.clipboardData.getData('text'));
    });
    ```

22. **Check Clipboard Content Type (Image or Text)**
    ```javascript
    navigator.clipboard.read().then(data => {
      data.forEach(item => {
        if (item.types.includes('image/png')) {
          console.log('Image is on the clipboard');
        } else if (item.types.includes('text/plain')) {
          console.log('Text is on the clipboard');
        }
      });
    });
    ```

23. **Set Custom Clipboard Content**
    ```javascript
    navigator.clipboard.writeText('Custom clipboard content').then(() => {
      console.log('Clipboard content set successfully!');
    });
    ```

24. **Add Text to Existing Clipboard Content**
    ```javascript
    navigator.clipboard.readText().then(text => {
      const updatedText = text + ' More text added';
      navigator.clipboard.writeText(updatedText);
    });
    ```

25. **Copy HTML to Clipboard**
    ```javascript
    function copyHTMLToClipboard(html) {
      const textarea = document.createElement('textarea');
      textarea.value = html;
      document.body.appendChild(textarea);
      textarea.select();
      document.execCommand('copy');
      document.body.removeChild(textarea);
    }
    copyHTMLToClipboard('<h1>Some HTML content</h1>');
    ```