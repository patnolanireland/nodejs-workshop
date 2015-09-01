##  Blocking I/O

What does it mean to block?

        var fs = require('fs');
        var fileContent = fs.readFileSync('productList.csv');
        console.log(fileContents);

Basically the console.log code doesn't run until after the file has been retrieved.

___

Why might this be bad?

Because our application can't do anything else until the file has been loaded. <!-- .element: class="fragment" data-fragmet-index="1" -->
