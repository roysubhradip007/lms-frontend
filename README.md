# LMS Frontend

### Setup instruction

1. clone the project
```
    git clone git@github.com:roysubhradip007/lms-frontend.git
```

2.move into the directory
```
    cd lms-frontend
```

3.install dependencies
```
    npm install
```

4.run the server
```
    npm run dev
```

### Setup instructions for tailwind

    [Tailwind official instruction doc] (https://tailwindcss.com/docs/installation)

1.install tailwind css
```
    npm install -D tailwindcss
```

2.create tailwind config file
```
    npx tailwindcss init
```

3.Add file extensions to tailwind config file in the content property
```
    "./src/**/*.{html,js,jsx,ts,tsx}"
```

4.Add the tailwind directives at the top of the `index.css` file
```
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
```

### Adding plugins and dependencies
```
    npm install @reduxjs/toolkit react-redux react-router-dom react-icons react-chartjs-2 chart.js daisyui axios react-hot-toast @tailwindcss/line-clamp
```

### confugure auto import sort eslint

1. install simple import sort
```
    npm i -D eslint-plugin-simple-import-sort
```

2. Add simple-import-sort plugin in `eslint.config.js`
```
    'simple-import-sort': simpleImportSort,
```

3. Add rule in "eslint.config.js"
```
    'simple-import-sort/imports': 'error',
```

4. To enable auto import sort on file save in vscode
    - open `settings.json`
    - add the following config
```
    "editor.codeActionsOnSave": {
        "source.fixAll.eslint":"explicit"
    }
```