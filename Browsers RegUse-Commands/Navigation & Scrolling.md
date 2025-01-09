## **Navigation & Scrolling**:

1. **Scroll to the Top of the Page**
   ```javascript
   window.scrollTo(0, 0);
   ```

2. **Scroll to the Bottom of the Page**
   ```javascript
   window.scrollTo(0, document.body.scrollHeight);
   ```

3. **Scroll to a Specific Element**
   ```javascript
   document.querySelector('#element-id').scrollIntoView();
   ```

4. **Smooth Scroll to the Top of the Page**
   ```javascript
   window.scrollTo({ top: 0, behavior: 'smooth' });
   ```

5. **Smooth Scroll to the Bottom of the Page**
   ```javascript
   window.scrollTo({ top: document.body.scrollHeight, behavior: 'smooth' });
   ```

6. **Scroll to a Specific Element Smoothly**
   ```javascript
   document.querySelector('#element-id').scrollIntoView({ behavior: 'smooth' });
   ```

7. **Scroll Horizontally to the Right**
   ```javascript
   window.scrollBy({ left: 100, behavior: 'smooth' });
   ```

8. **Scroll Horizontally to the Left**
   ```javascript
   window.scrollBy({ left: -100, behavior: 'smooth' });
   ```

9. **Scroll the Page by a Specific Amount**
   ```javascript
   window.scrollBy(0, 500); // Scrolls 500px down vertically
   ```

10. **Get Current Scroll Position**
    ```javascript
    let scrollPosition = window.scrollY || document.documentElement.scrollTop;
    console.log(scrollPosition);
    ```

11. **Scroll to the Top of an Element**
    ```javascript
    document.querySelector('#element-id').scrollIntoView({ block: 'start' });
    ```

12. **Enable Scroll Lock (Disable Scrolling)**
    ```javascript
    document.body.style.overflow = 'hidden';
    ```

13. **Disable Scroll Lock (Enable Scrolling)**
    ```javascript
    document.body.style.overflow = 'auto';
    ```

14. **Auto-Scroll an Element**
    ```javascript
    let element = document.querySelector('#element-id');
    element.scrollTop = element.scrollHeight;
    ```

15. **Scroll an Element by Specific Amount**
    ```javascript
    let element = document.querySelector('#element-id');
    element.scrollBy(0, 100); // Scrolls 100px down
    ```

16. **Scroll to a Specific Position in an Element**
    ```javascript
    let element = document.querySelector('#element-id');
    element.scrollTop = 200; // Scrolls to 200px down within the element
    ```

17. **Detect Scrolling Direction (Up or Down)**
    ```javascript
    window.addEventListener('scroll', function() {
        let direction = (this.scrollY > lastScrollPosition) ? 'down' : 'up';
        console.log(direction);
        lastScrollPosition = this.scrollY;
    });
    ```

18. **Scroll an Element into View if Not Visible**
    ```javascript
    let element = document.querySelector('#element-id');
    if (element.getBoundingClientRect().top < 0) {
        element.scrollIntoView({ behavior: 'smooth' });
    }
    ```

19. **Infinite Scroll Example (Load More Content)**
    ```javascript
    window.addEventListener('scroll', function() {
        if (window.innerHeight + window.scrollY >= document.body.scrollHeight) {
            // Load more content
            console.log('Loading more content...');
        }
    });
    ```

20. **Detect Scroll Position of an Element**
    ```javascript
    let element = document.querySelector('#element-id');
    let rect = element.getBoundingClientRect();
    console.log(rect.top); // Get the position relative to the viewport
    ```