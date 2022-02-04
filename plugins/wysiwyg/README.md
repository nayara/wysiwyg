<p align="center">
  <h1>Strapi Wysiwyg Plugin</h1>
</p>

<hr >
<h4 align="center">
tested on strapi v4.x

latest test: v4.0.6

<p align="center"> 
  The purpose of developing this plugin is to replace default WYSIWYG editor with CKEditor5.
</p>

<p align="center">
  This plugin has been develop from documentation reference:
  <a href="https://docs.strapi.io/developer-docs/latest/guides/registering-a-field-in-admin.html#creating-the-wysiwyg" rel="noopener">Creating the WYSIWYG</a>
</p>

## 📝 Table of Contents

- [🏁 Getting Started <a name = "getting_started"></a>](#-getting-started-)
  - [Strapi setup <a name="strapi_setup"></a>](#strapi-setup-)
  - [Editor configuration <a name="editor_config"></a>](#editor-configuration-)
    - [✍️ Authors <a name = "authors"></a>](#️-authors-)

## Prerequisites <a name="prerequisites"></a>

<hr />

Install plugin

- Go to the project path

  - `cd PROJECT/src/plugins`

- Clone the project

  - `git submodule add https://github.com/nayara/wysiwyg.git ./wysiwyg`

- Install dependencies

  - `yarn install`

# 🏁 Getting Started <a name = "getting_started"></a>

## Strapi setup <a name="strapi_setup"></a>

In order to activate plugin, you need to add the following settings to `PROJECT/config/plugins.js`

```js
module.exports = ({ env }) => ({
  ...
  elastic: {
    enabled: true,
    resolve: "./src/plugins/wysiwyg", // or the name of plugin folder
  },
  ...
});
```

## Editor configuration <a name="editor_config"></a>

- You can change the toolbar and other editor configuration at: `src/plugins/wysiwyg/admin/src/components/Editor/configuration.js`
- More info about customization options in:
  <a href="https://ckeditor.com/docs/ckeditor5/latest/builds/guides/integration/configuration.html" rel="noopener">CKEditor config</a>

### ✍️ Authors <a name = "authors"></a>

- [@cillaeslopes](https://github.com/cillaeslopes)
- [@nayara](https://github.com/nayara)
