1.  Task1
    Ans.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>User Login</title>
    <link rel="stylesheet" href="dist/output.css" />
  </head>
  <body class="flex min-h-screen items-center justify-center bg-gray-100">
    <div class="flex w-full max-w-3xl rounded-lg bg-white p-6 shadow-lg lg:p-8">
      <!-- Form Section -->
      <div class="w-full lg:w-2/3">
        <h2 class="mb-6 text-2xl font-bold text-gray-800">Login</h2>
        <form action="#" method="POST">
          <div class="mb-4">
            <label
              class="mb-2 block text-sm font-bold text-gray-600"
              for="username"
              >Username</label
            >
            <input
              class="w-full rounded-lg border px-3 py-2 text-gray-700 focus:outline-none focus:ring-2 focus:ring-blue-600"
              type="text"
              id="username"
              placeholder="Enter your username"
            />
          </div>
          <div class="mb-6">
            <label
              class="mb-2 block text-sm font-bold text-gray-600"
              for="password"
              >Password</label
            >
            <input
              class="w-full rounded-lg border px-3 py-2 text-gray-700 focus:outline-none focus:ring-2 focus:ring-blue-600"
              type="password"
              id="password"
              placeholder="Enter your password"
            />
          </div>
          <div class="flex items-center justify-between mb-6">
            <button
              class="focus:shadow-outline rounded bg-blue-600 px-4 py-2 font-bold text-white hover:bg-blue-700 focus:outline-none"
              type="button"
            >
              Sign In
            </button>
            <a
              class="inline-block align-baseline text-sm font-bold text-blue-600 hover:text-blue-800"
              href="#"
              >Forgot Password?</a
            >
          </div>
        </form>
        <!-- OR Divider -->
        <div class="mb-6 flex items-center justify-between">
          <hr class="w-full border-gray-300" />
          <span class="px-3 text-gray-500">OR</span>
          <hr class="w-full border-gray-300" />
        </div>
        <!-- Google Login Button -->
        <div>
          <button
            class="w-full flex items-center justify-center rounded-lg border border-gray-300 bg-white px-4 py-2 text-gray-700 shadow-sm hover:bg-gray-50 focus:outline-none focus:ring-2 focus:ring-blue-600"
          >
            <img
              src="https://img.icons8.com/color/16/000000/google-logo.png"
              class="mr-2"
              alt="Google Icon"
            />
            <span>Login with Google</span>
          </button>
        </div>
      </div>
      <!-- Image Section -->
      <div class="hidden lg:block lg:w-1/3">
        <img
          src="https://res.cloudinary.com/dhrbg2jbi/image/upload/v1724171795/close-up-portrait-young-beautiful-attractive-redhair-girl-happy-with-something-pointing-finger-blue-pastel-background-copy-space_sjcfw1.png"
          class="h-full w-auto rounded-lg"
          alt="Login Image"
        />
      </div>
    </div>
  </body>
</html>
```

2.  Task 2
    Ans.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Image Gallery</title>
    <link rel="stylesheet" href="dist/output.css" />
  </head>
  <body class="bg-gray-100">
    <div class="container mx-auto px-4 py-8">
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4">
        <img
          src="https://res.cloudinary.com/dhrbg2jbi/image/upload/v1724171795/close-up-portrait-young-beautiful-attractive-redhair-girl-happy-with-something-pointing-finger-blue-pastel-background-copy-space_sjcfw1.png"
          class="w-full h-auto object-cover rounded-lg shadow-md"
          alt="Image 1"
        />
        <img
          src="https://res.cloudinary.com/dhrbg2jbi/image/upload/v1724171795/close-up-portrait-young-beautiful-attractive-redhair-girl-happy-with-something-pointing-finger-blue-pastel-background-copy-space_sjcfw1.png"
          class="w-full h-auto object-cover rounded-lg shadow-md"
          alt="Image 2"
        />
        <img
          src="https://res.cloudinary.com/dhrbg2jbi/image/upload/v1724171795/close-up-portrait-young-beautiful-attractive-redhair-girl-happy-with-something-pointing-finger-blue-pastel-background-copy-space_sjcfw1.png"
          class="w-full h-auto object-cover rounded-lg shadow-md"
          alt="Image 3"
        />
        <img
          src="https://res.cloudinary.com/dhrbg2jbi/image/upload/v1724171795/close-up-portrait-young-beautiful-attractive-redhair-girl-happy-with-something-pointing-finger-blue-pastel-background-copy-space_sjcfw1.png"
          class="w-full h-auto object-cover rounded-lg shadow-md"
          alt="Image 4"
        />
        <!-- Add more images as needed -->
      </div>
    </div>
  </body>
</html>
```

3.  Task3
    Ans.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Dashboard</title>
    <link rel="stylesheet" href="dist/output.css" />
  </head>
  <body class="bg-gray-100 font-sans">
    <div class="flex h-screen">
      <!-- Sidebar -->
      <div class="w-1/4 bg-gray-800 text-white p-4">
        <h1 class="text-2xl font-bold mb-8">Dashboard</h1>
        <ul>
          <li class="mb-4">
            <a href="#" class="hover:bg-gray-700 block px-4 py-2 rounded"
              >Home</a
            >
          </li>
          <li class="mb-4">
            <a href="#" class="hover:bg-gray-700 block px-4 py-2 rounded"
              >Profile</a
            >
          </li>
          <li class="mb-4">
            <a href="#" class="hover:bg-gray-700 block px-4 py-2 rounded"
              >Settings</a
            >
          </li>
          <li class="mb-4">
            <a href="#" class="hover:bg-gray-700 block px-4 py-2 rounded"
              >Logout</a
            >
          </li>
        </ul>
      </div>

      <!-- Main Content -->
      <div class="w-3/4 p-8">
        <h2 class="text-xl font-semibold mb-6">Welcome to the Dashboard</h2>
        <div class="bg-white p-6 rounded-lg shadow-md">
          <!-- Dashboard content here -->
          <p>Your main content goes here.</p>
        </div>
      </div>
    </div>
  </body>
</html>
```
