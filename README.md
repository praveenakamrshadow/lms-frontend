# LMS Frontend

### Setup instructions

1. clone the project

```
    git clone https://github.com/praveenakamrshadow/lms-frontend.git
```

2. Move into the directory

```
    cd lms-frontend
```

3. Install dependencies

```
    npm i
```

4. Run the server

```
npm run dev
```

### How to setup tailwind in your project with vite [Link](https://tailwindcss.com/docs/guides/vite)

1. Install tailwind and other dependencies

```
npm install -D tailwindcss postcss autoprefixer
```

2. Create the `tailwind.config.js` file

```
npx tailwind init -p
```

3. Add the files and extensions to tailwind config in the content property

```

content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
],

```

4. Add the `@tailwind` directives for each of Tailwind’s layers to your `./src/index.css` file.
   
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

5. Start your build process
   
```
npm run dev
```

6. Start using Tailwind in your project

### Adding plugins and dependencies

```
    npm install @reduxjs/toolkit react-redux react-router-dom  react-icons react-chartjs-2 chart.js daisyui axios react-hot-toast @tailwindcss/line-clamp
```

### Adding auto import sort for eslint

1. Install the plugin
```
   npm i -D eslint-plugin-simple-import-sort
```

2. Add rule in `.eslintrc.js`
```
    'simple-import-sort/imports': 'error',
```

3. Add simpl-import-sort in the plugin array of `.eslintrc.js` file
```
plugins: [..., 'simple-import-sort']
```

4. Open `settings.json` in vscode configuration settings

5. Add the folowing line
```
    "editor.codeActionsOnSave": {
        "source.fixAll.eslint": true
    }

```