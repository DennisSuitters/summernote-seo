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
            element:'.summernote', // Element ID or Class used to Initialise Summernote
            notificationTime:2400, // Time to display Notifications
            keywordsElement:'#seoKeywords', // ID or Class of the Target Element to place content.
            keywordsElementType:'input', // input|html
            captionElement:'#seoCaption', // ID or Class of the Target Element to place content.
            captionElementType:'input', // input|html
            descriptionElement:'#seoDescription', // ID or Class of the Target Element to place content.
            descriptionElementType:'input', // input|html
            triggerInput:true, // Set this to True if like me you use AJAX to update single input fields
            action:'replace', // replace|append
            successClass:'alert alert-success',
            errorClass:'alert alert-danger',
            icon:'<i class="note-icon">[Your Icon]</i> <span class="caret"></span>',
    }
});
```

#### Thanks:
- To the Coder that wrote the Keyword Extraction Javascript. I can't remember where I got it from.
