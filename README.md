# summernote-keywords
A plugin for the [Summernote](https://github.com/summernote/summernote/) WYSIWYG editor.

summernote-keywords Extracts Keywords from the Editor Text, then places them in the chosen Element, either an Input Field, or HTML Area.asted Text can be Cleaned when Pasted into the Text Editor.

### Installation

#### 1. Include JS

Include the following code after Summernote:

```html
<script src="summernote-keywords.js"></script>
```

#### 2. Supported languages

Currently available in English!

#### 3. Summernote options

```javascript
$('.summernote').summernote({
    toolbar:[
        ['keywords',['keywords']], // The Button
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
    keywords:{
      element:'.summernote', // Class name of Summernote Instance
      time:2400, // Time to display Notification
      outElement:'#seoKeywords', // ID or Class of Element to place generated keywords
      outType:'input', // input|html Target Element Type
      triggerInput:true, // Set this to true, if like me you use ajax to update single fields
      action:'replace', // replace|append
      icon:'<i class="note-icon">/* Your SEO Icon */</i>'
    }
});
```

#### Thanks:
- To the Coder that wrote the Keyword Extraction Javascript. I can't remember where I got it from.
