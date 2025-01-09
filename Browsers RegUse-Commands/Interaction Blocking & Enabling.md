## **Interaction Blocking & Enabling**:

1. **Disable Right-Click on the Page**
   ```javascript
   document.addEventListener('contextmenu', function(e) {
       e.preventDefault();
   });
   ```

2. **Enable Right-Click on the Page (After Disabling)**
   ```javascript
   document.removeEventListener('contextmenu', function(e) {
       e.preventDefault();
   });
   ```

3. **Disable Text Selection on the Page**
   ```javascript
   document.body.style.userSelect = 'none';
   ```

4. **Enable Text Selection on the Page**
   ```javascript
   document.body.style.userSelect = 'auto';
   ```

5. **Disable All Links on the Page (Prevent Clicks)**
   ```javascript
   document.querySelectorAll('a').forEach(link => {
       link.addEventListener('click', function(e) {
           e.preventDefault();
       });
   });
   ```

6. **Enable All Links on the Page (Allow Clicks)**
   ```javascript
   document.querySelectorAll('a').forEach(link => {
       link.removeEventListener('click', function(e) {
           e.preventDefault();
       });
   });
   ```

7. **Disable Form Inputs on the Page**
   ```javascript
   document.querySelectorAll('input, textarea, button').forEach(input => {
       input.disabled = true;
   });
   ```

8. **Enable Form Inputs on the Page**
   ```javascript
   document.querySelectorAll('input, textarea, button').forEach(input => {
       input.disabled = false;
   });
   ```

9. **Disable All Buttons on the Page**
   ```javascript
   document.querySelectorAll('button').forEach(button => {
       button.disabled = true;
   });
   ```

10. **Enable All Buttons on the Page**
    ```javascript
    document.querySelectorAll('button').forEach(button => {
        button.disabled = false;
    });
    ```

11. **Block Keyboard Input (Disable Keyboard Events)**
    ```javascript
    document.addEventListener('keydown', function(e) {
        e.preventDefault();
    });
    ```

12. **Enable Keyboard Input (Allow Keyboard Events)**
    ```javascript
    document.removeEventListener('keydown', function(e) {
        e.preventDefault();
    });
    ```

13. **Disable Mouse Events (Prevent Mouse Clicks)**
    ```javascript
    document.body.style.pointerEvents = 'none';
    ```

14. **Enable Mouse Events (Allow Mouse Clicks)**
    ```javascript
    document.body.style.pointerEvents = 'auto';
    ```

15. **Block Page Scrolling Temporarily**
    ```javascript
    document.body.style.overflow = 'hidden';
    ```

16. **Enable Page Scrolling After Blocking**
    ```javascript
    document.body.style.overflow = 'auto';
    ```

17. **Disable All Dragging on the Page**
    ```javascript
    document.body.style.userSelect = 'none';
    document.body.style.pointerEvents = 'none';
    ```

18. **Enable All Dragging on the Page**
    ```javascript
    document.body.style.userSelect = 'auto';
    document.body.style.pointerEvents = 'auto';
    ```

19. **Disable All Form Submissions**
    ```javascript
    document.querySelectorAll('form').forEach(form => {
        form.addEventListener('submit', function(e) {
            e.preventDefault();
        });
    });
    ```

20. **Enable All Form Submissions**
    ```javascript
    document.querySelectorAll('form').forEach(form => {
        form.removeEventListener('submit', function(e) {
            e.preventDefault();
        });
    });
    ```