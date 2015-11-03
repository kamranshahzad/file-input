# File Input

JQuery plugin for preview browsed image


## Description

This plugin provides the better look for file input form field for all browsers. This plugin is easy to use and customize.


## Screenshot

![alt text](https://github.com/kamranshahzad/ImageUpload/assets/images/file-upload-screenshot.png "File Upload screenshot")

## Usage
### Dependencies:
* JQuery
* Twitter Bootstrap
* File Input (file-input.js)

Add file-input.js in your page
``` html
<link href="set_your_path/file-uploads.css" rel="stylesheet">
```

Add file-input.js in your page

``` html
<script src="set_your_path/file-input.js"></script>
```

Input field in your form
``` html
<input type="hidden" name="form_logo" id="form_logo" value="pic_123.png" >
<div class="form-group">
    <label for="form_logofile" class="col-sm-2 control-label">Logo File:</label>
    <div class="col-sm-10">
        <input type="file" name="person_form" id="form_logofile">
    </div>
</div>
```

Calling file input plugin
``` javascript
		$('#form_logofile').fileUpload({
            hiddenField: '#form_logo',
            showImage : true,
            imgSrc : 'assets/images/mCouponsLogoIcon58x58.png'
        });
```

	* `hiddenField` Form hidden field store the default image name.
	* `showImage`   Show image thumb if set 'true'. Show filename if set 'false'
	* `imgSrc`      Set default image thumb
	* `imageCaption` Set default image caption