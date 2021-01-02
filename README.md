# gatsby-plugin-heap

Gatsby plugin for Heap Analytics.

## Install

```sh
yarn add gatsby-plugin-heap
```
or
```sh
npm install gatsby-plugin-heap
```

## Usage

```sh
// In your gatsby-config.js
plugins: [
  {
    resolve: 'gatsby-plugin-heap',
    options: {
      appId: 'YOUR-APP-ID',
      enableOnDevMode: true // if 'false', heap will be fired on NODE_ENV=production only
    },
  },
],
```

## Heap App ID

You can find your ID in Account --> Manage --> Projects --> Environments.

If you made a new Heap account for your Gatsby project, sometimes you can't see your account management until after the installation step. If this is the case, Heap will have a code snippit it wants you to paste into the `</head>` tag. You do not need to paste the code snippet anywhere with this plugin. Your App ID is a unique string in that snippet. Once you add it to the plugin and run `gatsby develop`, refresh the Heap page to see your data and complete the installation process. 

