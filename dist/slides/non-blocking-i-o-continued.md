##  Non-blocking I/O

Essentially it makes use of a callback (don't call us we'll call you)

        var fs = require('fs');

        /* Read from the file system asynchronously */
        fs.readFile('/etc/passwd', function (err, data) {
            if (err) throw err;
                console.log('**** File Loaded Successfully ***');
                console.log(data);
        });

        /* This console.log will execute before the callback function above */
        console.log('Hi there I've been called before the callback');
