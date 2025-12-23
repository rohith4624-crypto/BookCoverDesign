# Ex.05 Book Front Cover Page Design
## Date:

## AIM:
To design a book front cover page using HTML and CSS.

## DESIGN STEPS:

### Step 1:
Create a Django Admin project.

### Step 2:
Create an app in the Django interface.

### Step 3:
Create a folder named 'static' in the app folder.

### Step 4:
Create a new HTML file in the static folder.

### Step 5:
Write the HTML code with relevant CSS properties.

### Step 6:
Choose the appropriate style and color scheme.

### Step 7:
Insert the images in their appropriate places.

### Step 8:
Publish the website in the LocalHost.

## PROGRAM:
```
BookCover.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Book Cover</title>
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: "Georgia", serif;
    }

    body {
      background: #111;
      height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .book-cover {
      width: 420px;
      height: 640px;
      position: relative;
      background: url('STR.jpg') center/cover no-repeat;
      box-shadow: 0 20px 40px rgba(0,0,0,0.6);
      border-radius: 6px;
      overflow: hidden;
    }

    /* Dark overlay for readability */
    .overlay {
      position: absolute;
      inset: 0;
      background: linear-gradient(
        to bottom,
        rgba(0,0,0,0.25) 0%,
        rgba(0,0,0,0.55) 60%,
        rgba(0,0,0,0.85) 100%
      );
    }

    .content {
      position: absolute;
      inset: 0;
      padding: 32px 28px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      color: #fff;
      z-index: 2;
    }

    .title {
      margin-top: 40px;
    }

    .title h1 {
      font-size: 38px;
      line-height: 1.1;
      letter-spacing: 1px;
      text-transform: uppercase;
    }

    .title span {
      display: block;
      margin-top: 8px;
      font-size: 14px;
      letter-spacing: 3px;
      opacity: 0.85;
    }

    .tagline {
      font-size: 16px;
      font-style: italic;
      max-width: 80%;
      opacity: 0.9;
    }

    .author {
      border-top: 1px solid rgba(255,255,255,0.3);
      padding-top: 16px;
      font-size: 18px;
      letter-spacing: 2px;
      text-transform: uppercase;
    }

    /* Optional spine effect */
    .spine {
      position: absolute;
      left: 0;
      top: 0;
      width: 18px;
      height: 100%;
      background: rgba(0,0,0,0.4);
    }

    @media (max-width: 480px) {
      .book-cover {
        transform: scale(0.9);
      }
    }
  </style>
</head>
<body>

  <div class="book-cover">
    <div class="spine"></div>
    <div class="overlay"></div>

    <div class="content">
      <div class="title">
        <h1>ATMAN</h1>
      </div>

      <div class="tagline">
        "A powerful line that hints at the soul of the story."
      </div>

      <div class="author">
        Fazil Ahamed A
      </div>
    </div>
  </div>

</body>
</html>

```

## OUTPUT:
<img width="1456" height="882" alt="Screenshot 2025-12-23 093907" src="https://github.com/user-attachments/assets/019f483f-7f68-4917-b896-a6e86ef965be" />


## RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
