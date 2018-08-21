<h1 align="center">It`s my Login page</h1>

<h2 align="center">Install with npm:</h2>

You can open my progect on Windows, Mac, or Linux by downloading npm version 6.2.0 and webpack version 4.16.5.

All plugins you need you can see in my package.json file.

For installation all environment run the following command:
```bash
npm install
```

In your package-lock.json should be the following scripts:
```bash
"dist": "webpack",
"dev": "webpack-dev-server --hot --open --inline"

In your webpack.config.js should be the following options:
  mode: 'development',
  entry: './src/index.js',
  output: {
    filename: 'main.js',
    path: path.resolve(__dirname, 'dist')
  },
  devServer: {
    contentBase: path.resolve(__dirname, 'dist'),
    hot: true
  },
  module: {
    rules:[
      {
        test: /\.less$/,
        use: ['style-loader', 'css-loader','less-loader']
      }
    ]
  },
  watch: true
```
### Get Started
  For pack you should run the following command:
```bash
  npm run dev
```
### Creating your own plugins and goods
If you create some plugin, I would be glad to open source it, and put it on my project.
If you have discovered some buggs or have some suggestion, feel free to tell about it.