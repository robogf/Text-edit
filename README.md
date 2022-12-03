# Text-edit

## Deployed Link

This is a deployed link of our application
![site](https://git.heroku.com/c00l-text-edit.git)

## Technologies Used

For this assignment we used our webpacks which allowed us to implement our webpack PWA.
Heroku- This was used to deploy our website.

## Summary

Through this application you are able to use a text editor and install it as PWA.

## Code Snippet

```JavaScript
new HtmlWebpackPlugin({
        template: './index.html',
        title: 'Text'
      }),

      new InjectManifest ({
        swSrc: './src-sw.js',
        swDest: 'src-sw.js'
      }),

      new WebpackPwaManifest({
        fingerprints: false,
        inject: true,
        name: 'text editor',
        short_name: 'textedit',
        description: 'write down your text',
        background_color: '#335ca3',
        theme_color: '#225ca3',
        start_url: '/',
        publicPath: '/',
        icons: [
          {
          src: path.resolve('src/images/logo.png'),
          sizes: [96,128,192,256,384,512],
          destination: path.join('assets', 'icons')
        },
      ],
      });

```

## Author Link

[LinkedIn](https://www.linkedin.com/in/angel-matias-01120b251/)
[GitHub] (https://github.com/robogf)
