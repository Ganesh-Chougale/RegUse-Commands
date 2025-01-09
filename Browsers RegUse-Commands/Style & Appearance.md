## **Style & Appearance**:

1. **Change Background Color**
   ```javascript
   document.body.style.backgroundColor = 'lightblue';
   ```

2. **Change Font Color**
   ```javascript
   document.body.style.color = 'red';
   ```

3. **Change Font Size**
   ```javascript
   document.body.style.fontSize = '20px';
   ```

4. **Change Font Family**
   ```javascript
   document.body.style.fontFamily = 'Arial, sans-serif';
   ```

5. **Change the Text of an Element**
   ```javascript
   document.querySelector('h1').innerText = 'New Text';
   ```

6. **Change an Element’s Border**
   ```javascript
   document.querySelector('div').style.border = '2px solid black';
   ```

7. **Set an Element’s Width**
   ```javascript
   document.querySelector('div').style.width = '500px';
   ```

8. **Set an Element’s Height**
   ```javascript
   document.querySelector('div').style.height = '300px';
   ```

9. **Add Shadow to an Element**
   ```javascript
   document.querySelector('div').style.boxShadow = '5px 5px 10px rgba(0,0,0,0.5)';
   ```

10. **Hide an Element**
    ```javascript
    document.querySelector('div').style.display = 'none';
    ```

11. **Show a Hidden Element**
    ```javascript
    document.querySelector('div').style.display = 'block';
    ```

12. **Make an Element Visible**
    ```javascript
    document.querySelector('div').style.visibility = 'visible';
    ```

13. **Hide an Element**
    ```javascript
    document.querySelector('div').style.visibility = 'hidden';
    ```

14. **Add CSS Class to an Element**
    ```javascript
    document.querySelector('div').classList.add('new-class');
    ```

15. **Remove CSS Class from an Element**
    ```javascript
    document.querySelector('div').classList.remove('old-class');
    ```

16. **Toggle CSS Class on an Element**
    ```javascript
    document.querySelector('div').classList.toggle('active');
    ```

17. **Change an Element’s Opacity**
    ```javascript
    document.querySelector('div').style.opacity = 0.5; // 0.0 to 1.0 range
    ```

18. **Apply Gradient Background**
    ```javascript
    document.body.style.background = 'linear-gradient(to right, red, yellow)';
    ```

19. **Add Border Radius (rounded corners)**
    ```javascript
    document.querySelector('div').style.borderRadius = '15px';
    ```

20. **Add Padding to an Element**
    ```javascript
    document.querySelector('div').style.padding = '20px';
    ```

21. **Change Page Layout (Grid or Flexbox)**
    ```javascript
    document.body.style.display = 'grid'; // Or 'flex'
    ```

22. **Add Hover Effect (CSS Style Change)**
    ```javascript
    document.querySelector('button').addEventListener('mouseenter', () => {
        document.querySelector('button').style.backgroundColor = 'blue';
    });
    document.querySelector('button').addEventListener('mouseleave', () => {
        document.querySelector('button').style.backgroundColor = '';
    });
    ```

23. **Center an Element Horizontally**
    ```javascript
    document.querySelector('div').style.margin = '0 auto';
    ```

24. **Center an Element Vertically**
    ```javascript
    document.querySelector('div').style.position = 'absolute';
    document.querySelector('div').style.top = '50%';
    document.querySelector('div').style.transform = 'translateY(-50%)';
    ```

25. **Make an Element Fixed in Position (Sticky)**
    ```javascript
    document.querySelector('div').style.position = 'fixed';
    ```

26. **Change an Element’s Z-Index**
    ```javascript
    document.querySelector('div').style.zIndex = 10;
    ```

27. **Set Maximum Width of an Element**
    ```javascript
    document.querySelector('div').style.maxWidth = '100%';
    ```

28. **Set Minimum Height of an Element**
    ```javascript
    document.querySelector('div').style.minHeight = '200px';
    ```

29. **Make an Element Transparent**
    ```javascript
    document.querySelector('div').style.backgroundColor = 'rgba(255, 255, 255, 0)';
    ```