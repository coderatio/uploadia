# Uploadia
A flexible PHP file upload library

# Download
``composer require coderatio/uploadia`` 

Or Clone this repo.

# Usage
```php
require 'vendor/autoload.php'; // if you downloaded via composer
// OR
require 'pathtouploadia/src/Uploadia.php';

$uploadia = new Coderatio\Uploadia\Uploadia();
$uploadia->setDir('uploads')
    ->setExtensions(['jpg', 'png', 'jpeg', 'gif'])
    ->setMaxSize(1); // In megabytes. 1MB
    
// There are several methods to use. e.g $uploadia->allowAllFormats(), $uploadia->sameName($bool) takes a boolean. e.t.c
    
if($uploadia->uploadFile('photo') {
     // photo is the file input name.
     // Get the uploaded file name or get error message.
     
     $uploadia->getUploadName(); // Returns uploaded file name;
     $uploadia->getMessage(); // Returns error messages
}
```

# Contribution
Fork the project and send pull request, email me via josiahoyahaya@gmail.com, find me on <a href="https://twitter.com/josiahoyahaya">Twitter</a> and say something about it anywhere possible.

# Licence
This project is licenced under MIT license.