# summernote-seo
A plugin for the [Summernote](https://github.com/summernote/summernote/) WYSIWYG editor.

summernote-seo Extracts Keywords, Captions (Highlighted), and Descriptions (Highlighted) from the Editor Text, then places them in the chosen Element, either an Input Field, or HTML Area.

#### Demo
[summernote-seo Demo](http://studiojunkyard.github.io/summernote-seo/)

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
            el:'.summernote', // Element ID or Class used to Initialise Summernote.
            notTime:2400, // Time to display Notifications.
            keyEl:'#seoKeywords', // ID or Class of the Target Element to place Keywords.
            keyElType:'input', // input|html
            capEl:'#seoCaption', // ID or Class of the Target Element to place Caption.
            capElType:'input', // input|html
            desEl:'#seoDescription', // ID or Class of the Target Element to place Description.
            desElType:'input', // input|html
            triggerInput:true, // Set this to True if like me you use AJAX to update single fields
            action:'replace', // replace|append Replace or Append Content.
            successClass:'alert alert-success',
            errorClass:'alert alert-danger',
            icon:'<i class="note-icon">[Your Icon]</i> <span class="caret"></span>',
    }
});
```

#### Thanks:
- To the Coder that wrote the Keyword Extraction Javascript. I can't remember where I got it from.
