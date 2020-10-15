CKEditor 5 Classic Editor Build - Complete (Most Plugins) 
========================================

The classic editor build for CKEditor 5. Read more about the [classic editor build](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/overview.html#classic-editor) and see the [demo](https://ckeditor.com/docs/ckeditor5/latest/examples/builds/classic-editor.html).

![CKEditor 5 classic editor build screenshot](https://c.cksource.com/a/1/img/npm/ckeditor5-build-classic.png)

## Plugins Included (so far)
* [Essentials](https://www.npmjs.com/package/@ckeditor/ckeditor5-essentials)
* [Adapter Ckfinder](https://www.npmjs.com/package/@ckeditor/ckeditor5-adapter-ckfinder)
	* Upload Adapter
* [Autoformat](https://www.npmjs.com/package/@ckeditor/ckeditor5-autoformat)
* [Basic Styles](https://www.npmjs.com/package/@ckeditor/ckeditor5-basic-styles)
	* Bold
	* Italic
	* Underline
* [BlockQuote](https://www.npmjs.com/package/@ckeditor/ckeditor5-block-quote)
* [CKFinder](https://www.npmjs.com/package/@ckeditor/ckeditor5-ckfinder)
* [EasyImage](https://www.npmjs.com/package/@ckeditor/ckeditor5-easy-image)
* [Heading](https://www.npmjs.com/package/@ckeditor/ckeditor5-heading)
* [Image](https://www.npmjs.com/package/@ckeditor/ckeditor5-image)
	* Image
	* Image Caption
	* Image Style
	* Image Toolbar
	* Image Upload
* [Link](https://www.npmjs.com/package/@ckeditor/ckeditor5-link)
* [List](https://www.npmjs.com/package/@ckeditor/ckeditor5-list)
* [MediaEmbed](https://www.npmjs.com/package/@ckeditor/ckeditor5-media-embed)
* [Paragraph](https://www.npmjs.com/package/@ckeditor/ckeditor5-paragraph)
* [PasteFromOffice](https://www.npmjs.com/package/@ckeditor/ckeditor5-paste-from-office)
* [Table](https://www.npmjs.com/package/@ckeditor/ckeditor5-table)
	* Table
	* Table Toolbar
* [Alignment](https://www.npmjs.com/package/@ckeditor/ckeditor5-alignment)
* [Highlight](https://www.npmjs.com/package/@ckeditor/ckeditor5-highlight)

## Documentation

See:

* [Installation](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/integration/installation.html) for how to install this package and what it contains.
* [Basic API](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/integration/basic-api.html) for how to create an editor and interact with it.
* [Configuration](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/integration/configuration.html) for how to configure the editor.


## Quick start

First, install the build from npm:

```bash
npm install --save ckeditor5-build-classic-complete
```

And use it in your website:

```html
<div id="editor">
	<p>This is the editor content.</p>
</div>
<script src="./node_modules/ckeditor5-build-classic-complete/build/ckeditor.js"></script>
<script>
	ClassicEditor
		.create( document.querySelector( '#editor' ) )
		.then( editor => {
			window.editor = editor;
		} )
		.catch( err => {
			console.error( err.stack );
		} );
</script>
```

Or in your JavaScript application:

```js
import ClassicEditor from 'ckeditor5-build-classic-complete';

// Or using the CommonJS version:
// const ClassicEditor = require( 'ckeditor5-build-classic-complete' );

ClassicEditor
	.create( document.querySelector( '#editor' ) )
	.then( editor => {
		window.editor = editor;
	} )
	.catch( err => {
		console.error( err.stack );
	} );
```

**Note:** If you are planning to integrate CKEditor 5 deep into your application, it is actually more convenient and recommended to install and import the source modules directly (like it happens in `ckeditor.js`). Read more in the [Advanced setup guide](https://ckeditor.com/docs/ckeditor5/latest/builds/guides/integration/advanced-setup.html).

## License

Licensed under the terms of [GNU General Public License Version 2 or later](http://www.gnu.org/licenses/gpl.html). For full details about the license, please check the `LICENSE.md` file.
