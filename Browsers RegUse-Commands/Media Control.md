## **Media Control**:

1. **Play a Video**
   ```javascript
   document.querySelector('video').play();
   ```

2. **Pause a Video**
   ```javascript
   document.querySelector('video').pause();
   ```

3. **Set Video Playback Speed**
   ```javascript
   document.querySelector('video').playbackRate = 2;
   ```

4. **Mute a Video**
   ```javascript
   document.querySelector('video').muted = true;
   ```

5. **Unmute a Video**
   ```javascript
   document.querySelector('video').muted = false;
   ```

6. **Set Volume of a Video**
   ```javascript
   document.querySelector('video').volume = 0.5; // 0.0 to 1.0 range
   ```

7. **Get Current Time of Video**
   ```javascript
   console.log(document.querySelector('video').currentTime);
   ```

8. **Set Current Time of Video**
   ```javascript
   document.querySelector('video').currentTime = 30; // 30 seconds
   ```

9. **Get Duration of Video**
   ```javascript
   console.log(document.querySelector('video').duration);
   ```

10. **Loop a Video**
    ```javascript
    document.querySelector('video').loop = true;
    ```

11. **Skip to the Next Video in a Playlist (if applicable)**
    ```javascript
    document.querySelector('video').nextElementSibling.play();
    ```

12. **Load Video (to reload a video)**
    ```javascript
    document.querySelector('video').load();
    ```

13. **Show/Hide Video Controls**
    ```javascript
    document.querySelector('video').controls = true;  // Show controls
    document.querySelector('video').controls = false; // Hide controls
    ```

14. **Get All Video Elements**
    ```javascript
    const videos = document.querySelectorAll('video');
    console.log(videos);
    ```

15. **Pause All Videos on the Page**
    ```javascript
    const videos = document.querySelectorAll('video');
    videos.forEach(video => video.pause());
    ```

16. **Mute All Videos on the Page**
    ```javascript
    const videos = document.querySelectorAll('video');
    videos.forEach(video => video.muted = true);
    ```

17. **Change Source of Video**
    ```javascript
    document.querySelector('video').src = 'new-video.mp4';
    ```

18. **Play Audio in Background**
    ```javascript
    const audio = new Audio('background-audio.mp3');
    audio.play();
    ```

19. **Pause Audio**
    ```javascript
    const audio = new Audio('background-audio.mp3');
    audio.pause();
    ```