# Tailwind CSS Integration 

This instruction is providing step-by-step guide for import Tailwind CSS in Project.

Download this repository starter pack code and run below command for import Tailwind CSS directly in your project.

```bash
npm install
```

## Option 1: Quick Setup

1. Add the following script tag to your HTML file to import Tailwind CSS directly from the CDN:
   ```html
   <script src="https://cdn.tailwindcss.com"></script>
   ```

## Option 2: Installation and Setup


1. **Install Node:**
Ensure that Node.js is installed on your machine. You can check if Node.js is installed by running the following command in your terminal:
   ```bash
   npm -v
   ```
   If Node.js is not installed, download and install it from https://nodejs.org/.

2. **Run Terminal Commands:**
In your project directory, run the following commands in the terminal:

   ```bash
   npm install -D tailwindcss postcss autoprefixer vite
   npx tailwindcss init -p
   ```
3. **Install Tailwind CSS Extension:**
Install the Tailwind CSS extension for your code editor. Choose an extension with a high number of downloads for better support.

4. **Configure Tailwind CSS:**
Open the `tailwind.config.js` file and add the following line to the `content` array:

   ```html
   content : ["*"]
   ```
5. **Update Package.json:**
Add the following script key to your `package.json` file:

   ```html
   "scripts": {
      "start" : "vite"
   }
   ```
6. **Create Main CSS File:**
Create a `main.css` file and add the following content:

   ```html
   @tailwind base;
   @tailwind components;
   @tailwind utilities;
   ```
7. **Link Main CSS File:**
Link the `main.css` file in your main HTML file.

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
      <meta charset="UTF-8">
      <meta name="viewport" content="width=device-width, initial-scale=1.0">
      <title>Document</title>
      <link rel="stylesheet" href="main.css">
   </head>
   <body>
      <div class="bg-green-500">Sample HTML Text</div>
   </body>
   </html>
   ```

## Running the Project
To start your project, run the following command in the terminal:

```bash
npm run start
```



