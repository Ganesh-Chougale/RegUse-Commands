## **Information Extraction**:

1. **Get the Title of the Current Page**
   ```javascript
   const pageTitle = document.title;
   console.log(pageTitle);
   ```

2. **Get the Current URL of the Page**
   ```javascript
   const currentURL = window.location.href;
   console.log(currentURL);
   ```

3. **Get All Links on the Page**
   ```javascript
   const allLinks = Array.from(document.querySelectorAll('a')).map(link => link.href);
   console.log(allLinks);
   ```

4. **Get All Image Sources on the Page**
   ```javascript
   const allImages = Array.from(document.querySelectorAll('img')).map(img => img.src);
   console.log(allImages);
   ```

5. **Get All Text Content from the Page**
   ```javascript
   const pageText = document.body.innerText;
   console.log(pageText);
   ```

6. **Get All Form Inputs Values on the Page**
   ```javascript
   const formInputs = Array.from(document.querySelectorAll('input, select, textarea'))
                           .map(input => input.value);
   console.log(formInputs);
   ```

7. **Get the Current User-Agent of the Browser**
   ```javascript
   const userAgent = navigator.userAgent;
   console.log(userAgent);
   ```

8. **Get All the Cookies for the Page**
   ```javascript
   const cookies = document.cookie;
   console.log(cookies);
   ```

9. **Get the Width and Height of the Window**
   ```javascript
   const windowWidth = window.innerWidth;
   const windowHeight = window.innerHeight;
   console.log(`Width: ${windowWidth}, Height: ${windowHeight}`);
   ```

10. **Get All Meta Tags from the Page**
    ```javascript
    const metaTags = Array.from(document.getElementsByTagName('meta')).map(meta => meta.name);
    console.log(metaTags);
    ```

11. **Get the Number of Paragraphs on the Page**
    ```javascript
    const paragraphCount = document.querySelectorAll('p').length;
    console.log(paragraphCount);
    ```

12. **Get the Current Date and Time**
    ```javascript
    const currentDateTime = new Date();
    console.log(currentDateTime);
    ```

13. **Get the First Image on the Page**
    ```javascript
    const firstImage = document.querySelector('img').src;
    console.log(firstImage);
    ```

14. **Get the InnerHTML of a Specific Element by ID**
    ```javascript
    const elementHTML = document.getElementById('elementID').innerHTML;
    console.log(elementHTML);
    ```

15. **Get the Text Content of a Specific Element by Class**
    ```javascript
    const elementText = document.querySelector('.elementClass').innerText;
    console.log(elementText);
    ```

16. **Get All Comments on the Page**
    ```javascript
    const comments = Array.from(document.createTreeWalker(document, NodeFilter.SHOW_COMMENT))
                          .map(comment => comment.nodeValue);
    console.log(comments);
    ```

17. **Get the Title and URL of All Anchor Tags**
    ```javascript
    const anchorData = Array.from(document.querySelectorAll('a')).map(anchor => ({
        title: anchor.title,
        href: anchor.href
    }));
    console.log(anchorData);
    ```

18. **Get the Font Size of a Specific Element**
    ```javascript
    const fontSize = window.getComputedStyle(document.getElementById('elementID')).fontSize;
    console.log(fontSize);
    ```

19. **Get the Number of Images on the Page**
    ```javascript
    const imageCount = document.querySelectorAll('img').length;
    console.log(imageCount);
    ```

20. **Get the Current Network Connection Type**
    ```javascript
    const connectionType = navigator.connection.effectiveType;
    console.log(connectionType);
    ```