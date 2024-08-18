1.  Create an image gallery that holds multiple images.
    Ans.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Image Gallery</title>
    <style>
      .gallery {
        display: flex;
        flex-wrap: wrap;
        gap: 10px;
      }

      .gallery img {
        width: 200px;
        height: 150px;
        object-fit: cover;
        border-radius: 10px;
      }
    </style>
  </head>
  <body>
    <div class="gallery">
      <img
        src="https://cdn.pixabay.com/photo/2024/08/05/21/19/lion-8947711_1280.jpg"
        alt="Image 1"
      />
      <img
        src="https://cdn.pixabay.com/photo/2018/03/04/17/23/tiger-3198598_640.jpg"
        alt="Image 2"
      />
      <img
        src="https://cdn.pixabay.com/photo/2024/02/19/13/50/monkeys-8583435_960_720.jpg"
        alt="Image 3"
      />
      <img
        src="https://media.istockphoto.com/id/623930140/photo/monkey-on-stupa-at-swayambhunath-temple-iconic-landmark-kathmandu-nepal.jpg?s=2048x2048&w=is&k=20&c=Jh5P311I18O_zWLsI2Mef2D9ay_3opBUpnndOfEPUhQ="
        alt="Image 4"
      />
    </div>
  </body>
</html>
```

2. Use video and audio tags to display video and audio with the playback, audio controls.
   Ans.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Video and Audio</title>
  </head>
  <body>
    <h2>Video</h2>
    <video width="320" height="240" controls>
      <source
        src="https://media.istockphoto.com/id/1585668662/video/interior-designer-working-on-new-house-design-project-in-office-choosing-flooring-and.mp4?s=mp4-640x640-is&k=20&c=Zqvnple6V8UYUDe9lxRNo2Wv9l5VgaWbyVG_C8zwPow="
        type="video/mp4"
      />
      Your browser does not support the video tag.
    </video>

    <h2>Audio</h2>
    <audio controls>
      <source
        src="https://commondatastorage.googleapis.com/codeskulptor-demos/DDR_assets/Kangaroo_MusiQue_-_The_Neverwritten_Role_Playing_Game.mp3"
        type="audio/mp3"
      />
      Your browser does not support the audio element.
    </audio>
  </body>
</html>
```

3. Modify the previous assignment so that the audio and video play automatically as the page is loaded, and they should play infinitely
   Ans.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Video and Audio</title>
  </head>
  <body>
    <h2>Video</h2>
    <video width="320" height="240" controls autoplay loop>
      <source
        src="https://media.istockphoto.com/id/1585668662/video/interior-designer-working-on-new-house-design-project-in-office-choosing-flooring-and.mp4?s=mp4-640x640-is&k=20&c=Zqvnple6V8UYUDe9lxRNo2Wv9l5VgaWbyVG_C8zwPow="
        type="video/mp4"
      />
      Your browser does not support the video tag.
    </video>

    <h2>Audio</h2>
    <audio controls autoplay loop>
      <source
        src="https://commondatastorage.googleapis.com/codeskulptor-demos/DDR_assets/Kangaroo_MusiQue_-_The_Neverwritten_Role_Playing_Game.mp3"
        type="audio/mp3"
      />
      Your browser does not support the audio element.
    </audio>
  </body>
</html>
```

4. Use iframe to embed the PhysicsWallah Wikipedia page properly.
   Ans.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>PhysicsWallah Wikipedia</title>
  </head>
  <body>
    <h2>PhysicsWallah Wikipedia Page</h2>
    <iframe
      src="https://en.wikipedia.org/wiki/PhysicsWallah"
      width="100%"
      height="500px"
    ></iframe>
  </body>
</html>
```

5. Create a sign-up and sign-in form with proper validation.
   a. Sign-up form should have fields for first name, last name, email, password, confirm password, age, gender, and agree to terms and conditions (at a minimum).
   b. Sign-in form should have fields for email and password.
   Ans.
   Sign Up

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Sign Up</title>
    <script>
      function validateSignUpForm() {
        let firstName = document.forms["signUpForm"]["firstName"].value;
        let lastName = document.forms["signUpForm"]["lastName"].value;
        let email = document.forms["signUpForm"]["email"].value;
        let password = document.forms["signUpForm"]["password"].value;
        let confirmPassword =
          document.forms["signUpForm"]["confirmPassword"].value;
        let age = document.forms["signUpForm"]["age"].value;

        if (firstName.length < 3 || lastName.length < 3) {
          alert("First name and last name must be at least 3 characters long.");
          return false;
        }
        if (!email.includes("@")) {
          alert("Please enter a valid email address.");
          return false;
        }
        if (password !== confirmPassword) {
          alert("Passwords do not match.");
          return false;
        }
        if (age < 0 || age > 150) {
          alert("Please enter a valid age.");
          return false;
        }
        return true;
      }
    </script>
  </head>
  <body>
    <h2>Sign Up</h2>
    <form name="signUpForm" onsubmit="return validateSignUpForm()">
      <label for="firstName">First Name:</label>
      <input type="text" id="firstName" name="firstName" required /><br /><br />

      <label for="lastName">Last Name:</label>
      <input type="text" id="lastName" name="lastName" required /><br /><br />

      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required /><br /><br />

      <label for="password">Password:</label>
      <input
        type="password"
        id="password"
        name="password"
        required
      /><br /><br />

      <label for="confirmPassword">Confirm Password:</label>
      <input
        type="password"
        id="confirmPassword"
        name="confirmPassword"
        required
      /><br /><br />

      <label for="age">Age:</label>
      <input type="number" id="age" name="age" required /><br /><br />

      <label for="gender">Gender:</label>
      <select id="gender" name="gender" required>
        <option value="male">Male</option>
        <option value="female">Female</option>
        <option value="other">Other</option></select
      ><br /><br />

      <input type="checkbox" id="terms" name="terms" required />
      <label for="terms">I agree to the terms and conditions</label><br /><br />

      <input type="submit" value="Sign Up" />
    </form>
  </body>
</html>
```

    Sign in

````html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Sign In</title>
    <script>
      function validateSignInForm() {
        let email = document.forms["signInForm"]["email"].value;
        let password = document.forms["signInForm"]["password"].value;

        if (!email.includes("@")) {
          alert("Please enter a valid email address.");
          return false;
        }
        if (password.length < 6) {
          alert("Password must be at least 6 characters long.");
          return false;
        }
        return true;
      }
    </script>
  </head>
  <body>
    <h2>Sign In</h2>
    <form name="signInForm" onsubmit="return validateSignInForm()">
      <label for="email">Email:</label>
      <input type="email" id="email" name="email" required /><br /><br />

      <label for="password">Password:</label>
      <input
        type="password"
        id="password"
        name="password"
        required
      /><br /><br />

      <input type="submit" value="Sign In" />
    </form>
  </body>
</html>
```
````
