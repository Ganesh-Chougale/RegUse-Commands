## **Image Manipulation**:

1. **Change Image Source**
   ```javascript
   document.querySelector('img').src = 'new-image.jpg';
   ```

2. **Set Image Width**
   ```javascript
   document.querySelector('img').style.width = '300px';
   ```

3. **Set Image Height**
   ```javascript
   document.querySelector('img').style.height = '200px';
   ```

4. **Change Image Alt Text**
   ```javascript
   document.querySelector('img').alt = 'New Alt Text';
   ```

5. **Add a Border to an Image**
   ```javascript
   document.querySelector('img').style.border = '5px solid black';
   ```

6. **Rotate an Image**
   ```javascript
   document.querySelector('img').style.transform = 'rotate(45deg)';
   ```

7. **Apply a Filter to an Image**
   ```javascript
   document.querySelector('img').style.filter = 'grayscale(100%)';
   ```

8. **Make an Image Round (Circular)**
   ```javascript
   document.querySelector('img').style.borderRadius = '50%';
   ```

9. **Flip an Image Horizontally**
   ```javascript
   document.querySelector('img').style.transform = 'scaleX(-1)';
   ```

10. **Flip an Image Vertically**
    ```javascript
    document.querySelector('img').style.transform = 'scaleY(-1)';
    ```

11. **Change Image Opacity**
    ```javascript
    document.querySelector('img').style.opacity = 0.5; // 0.0 to 1.0 range
    ```

12. **Replace All Images on the Page with a New Image**
    ```javascript
    document.querySelectorAll('img').forEach(img => {
        img.src = 'new-image.jpg';
    });
    ```

13. **Hide All Images on the Page**
    ```javascript
    document.querySelectorAll('img').forEach(img => {
        img.style.display = 'none';
    });
    ```

14. **Show All Hidden Images on the Page**
    ```javascript
    document.querySelectorAll('img').forEach(img => {
        img.style.display = 'block';
    });
    ```

15. **Set Image Border Radius**
    ```javascript
    document.querySelector('img').style.borderRadius = '15px';
    ```

16. **Make Image Transparent**
    ```javascript
    document.querySelector('img').style.opacity = 0; // Fully transparent
    ```

17. **Make Image Greyscale**
    ```javascript
    document.querySelector('img').style.filter = 'grayscale(100%)';
    ```

18. **Make Image Sepia**
    ```javascript
    document.querySelector('img').style.filter = 'sepia(100%)';
    ```

19. **Make Image Blurry**
    ```javascript
    document.querySelector('img').style.filter = 'blur(5px)';
    ```

20. **Animate Image Size Change**
    ```javascript
    document.querySelector('img').style.transition = 'width 0.5s, height 0.5s';
    document.querySelector('img').style.width = '400px';
    document.querySelector('img').style.height = '250px';
    ```

21. **Add a Shadow Effect to an Image**
    ```javascript
    document.querySelector('img').style.boxShadow = '10px 10px 15px rgba(0, 0, 0, 0.5)';
    ```