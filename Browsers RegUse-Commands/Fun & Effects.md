## **Fun & Effects**:

1. **Shake the Page**
   ```javascript
   document.body.style.position = 'relative';
   let shake = 0;
   const shakeInterval = setInterval(() => {
     if (shake < 10) {
       document.body.style.left = (Math.random() * 10 - 5) + 'px';
       document.body.style.top = (Math.random() * 10 - 5) + 'px';
       shake++;
     } else {
       clearInterval(shakeInterval);
       document.body.style.left = '0px';
       document.body.style.top = '0px';
     }
   }, 50);
   ```

2. **Toggle Dark Mode**
   ```javascript
   document.body.classList.toggle('dark-mode');
   ```
   *Note: Add relevant CSS for `.dark-mode` for actual effect.*

3. **Flash the Screen with Color**
   ```javascript
   const flash = document.createElement('div');
   flash.style.position = 'fixed';
   flash.style.top = '0';
   flash.style.left = '0';
   flash.style.width = '100%';
   flash.style.height = '100%';
   flash.style.backgroundColor = 'red';
   flash.style.opacity = '0.5';
   document.body.appendChild(flash);
   setTimeout(() => document.body.removeChild(flash), 500);
   ```

4. **Play a Sound when Clicking**
   ```javascript
   document.body.addEventListener('click', () => {
     const audio = new Audio('https://www.soundjay.com/button/beep-07.wav');
     audio.play();
   });
   ```

5. **Random Background Color Change**
   ```javascript
   setInterval(() => {
     document.body.style.backgroundColor = '#' + Math.floor(Math.random()*16777215).toString(16);
   }, 1000);
   ```

6. **Random Text Color Change**
   ```javascript
   setInterval(() => {
     document.body.style.color = '#' + Math.floor(Math.random()*16777215).toString(16);
   }, 1000);
   ```

7. **Scroll the Page Randomly**
   ```javascript
   setInterval(() => {
     window.scrollTo(Math.random() * document.body.scrollWidth, Math.random() * document.body.scrollHeight);
   }, 1000);
   ```

8. **Change All Links Color on Hover**
   ```javascript
   const links = document.querySelectorAll('a');
   links.forEach(link => {
     link.addEventListener('mouseover', () => {
       link.style.color = 'orange';
     });
     link.addEventListener('mouseout', () => {
       link.style.color = '';
     });
   });
   ```

9. **Confetti Effect on Page Load**
   ```javascript
   const confetti = document.createElement('div');
   confetti.style.position = 'absolute';
   confetti.style.top = '50%';
   confetti.style.left = '50%';
   confetti.style.width = '100px';
   confetti.style.height = '100px';
   confetti.style.background = 'url(https://www.gstatic.com/webp/gallery/2.jpg)';
   confetti.style.animation = 'confetti-animation 3s ease-in-out infinite';
   document.body.appendChild(confetti);
   ```

10. **Force Zoom In/Out on the Page**
    ```javascript
    document.body.style.zoom = '150%'; // Zoom In
    // Or to Zoom Out
    document.body.style.zoom = '50%';
    ```

11. **Bounce an Element**
    ```javascript
    const element = document.getElementById('elementID');
    element.style.position = 'relative';
    let bounceCount = 0;
    const bounceInterval = setInterval(() => {
      if (bounceCount < 10) {
        element.style.top = (Math.random() * 10 - 5) + 'px';
        bounceCount++;
      } else {
        clearInterval(bounceInterval);
        element.style.top = '0px';
      }
    }, 100);
    ```

12. **Snowfall Effect**
    ```javascript
    const snowflakes = [];
    const snowfall = () => {
      let snowflake = document.createElement('div');
      snowflake.style.position = 'absolute';
      snowflake.style.top = '0';
      snowflake.style.left = Math.random() * window.innerWidth + 'px';
      snowflake.style.width = '10px';
      snowflake.style.height = '10px';
      snowflake.style.backgroundColor = 'white';
      snowflake.style.borderRadius = '50%';
      snowflake.style.animation = 'fall 5s linear infinite';
      document.body.appendChild(snowflake);
      snowflakes.push(snowflake);
    };
    setInterval(snowfall, 200);
    ```

13. **Rotate the Page**
    ```javascript
    document.body.style.transition = 'transform 1s';
    document.body.style.transform = 'rotate(360deg)';
    ```

14. **Make an Element Grow on Hover**
    ```javascript
    document.querySelector('#elementID').addEventListener('mouseenter', () => {
      document.querySelector('#elementID').style.transform = 'scale(1.5)';
    });
    document.querySelector('#elementID').addEventListener('mouseleave', () => {
      document.querySelector('#elementID').style.transform = 'scale(1)';
    });
    ```

15. **Random Character Typing Effect**
    ```javascript
    const target = document.getElementById('text');
    const text = 'Hello, World!';
    let i = 0;
    const typingEffect = setInterval(() => {
      if (i < text.length) {
        target.textContent += text.charAt(i);
        i++;
      } else {
        clearInterval(typingEffect);
      }
    }, 100);
    ```

16. **Randomly Change Font Family of the Page**
    ```javascript
    const fontFamilies = ['Arial', 'Verdana', 'Courier', 'Georgia', 'Times New Roman'];
    setInterval(() => {
      document.body.style.fontFamily = fontFamilies[Math.floor(Math.random() * fontFamilies.length)];
    }, 2000);
    ```