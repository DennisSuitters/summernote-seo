# summernote-seo
A plugin for the [Summernote](https://github.com/summernote/summernote/) WYSIWYG editor.

summernote-seo Extracts Keywords, Captions (Highlighted), and Descriptions (Highlighted) from the Editor Text, then places them in the chosen Element, either an Input Field, or HTML Area.

### Installation

#### 1. Include JS

Include the following code after Summernote:

```html
<script src="summernote-seo.js"></script>
```

#### 2. Supported languages

Currently available in English!

#### 3. Summernote options

```javascript
$('.summernote').summernote({
    toolbar:[
        ['seo',['seo']], // The Button
        ['style',['style']],
        ['font',['bold','italic','underline','clear']],
        ['fontname',['fontname']],
        ['color',['color']],
        ['para',['ul','ol','paragraph']],
        ['height',['height']],
        ['table',['table']],
        ['insert',['media','link','hr']],
        ['view',['fullscreen','codeview']],
        ['help',['help']]
    ],
    seo:{
    }
});
```

#### Thanks:
- To the Coder that wrote the Keyword Extraction Javascript. I can't remember where I got it from.
