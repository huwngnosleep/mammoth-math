This is an extended version of npm package "mammoth". I added an indicator for **OMML** element read called ```</thisismath>```. This indicator can be filled by others external math reader. Such as I am using "word-math" for my projects.

# Usage

```
const mammoth = require('mammoth-math')
const word = require('word-math');

let data = await mammoth.convertToHtml({ path: docxFile.path })

const mathData = word.readFile(docxFile.path).maths
for (const mathElement of mathData) {
  data.value = data.value.replace(/&lt;\/thisismath&gt;/, mathElement)
}

console.log(data.value)
```

#   m a m m o t h - m a t h  
 #   m a m m o t h - m a t h  
 #   m a m m o t h - m a t h  
 