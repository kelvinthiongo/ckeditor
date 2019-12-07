Standard CKEditor 4
==========

Copyright (c) 2003-2019, CKSource - Frederico Knabben. All rights and credits to:
http://ckeditor.com - See LICENSE.md for license information.

Standard CKEditor 4 is a free customized ckeditor that consists of the most standard features and characteristics. Kelvin Thiongo Adjusted the ckeditor by adding some features such as Keystrokes including CTRL S for saving, ALT 1 -> H1, ALT 2 -> H2 ... You literally rearly need to add anything my fren...

# Documentation

## Features

 1. **Keystrokes (Short hand operations).** The free standard CKEditor 4 has a plugin called keystrokes that enables common 	operations such as CTRL + S for saving the document into your server. Here's the list:
 	> CTRL + S: Save | 
	> ALT + 1: Heading 1 | 
	> ALT + 2: Heading 2 | 
	> ALT + 3: Heading 3 | 
	> ALT + 4: Heading 4 | 
	> ALT + 5: Heading 5 | 
	> ALT + 6: Heading 6 | 
	> ALT + 7: Paragraph(Normal)

 2. **Image Customization.** This enables to select an image from your local files or input URL. Additionally, it offers room for setting the dimentions of the image. Miracurously, your can align the image using this feature. This image is pasisted to the database inform of base64. It is not recommended to store this data into your database as it may flood your database. You should therefore pluck out this base64 blob in your server side, convert base64 image to file format and replace this with img tag and src attribute pointing to where you store the image.

 3. **Embedding Youtube Video.** You just enter the url of the youtube video an iframe of the video is inserted. You can click the red play button of youtube and the video plays within the editor.

 4. **Emojis.** You can as well add emojis to your content.

 5. **Basic Stylings.** It has basic styles such as Italics, bold, tables, spellcheckers, Special characters.

 6. **No Source button.** It is always not recommended to leave capabilty of editing the source on the users' hands. Reason is that they can alter the code which would inturn disorient your page in the event of displaying their content. Therefore Standard CKEditor 4 has disabled this button for you.

 7. **Font Awesome Icons.** It is possible with this package to insert font awsome icons to your content. 

## Installation

Installing Standard CKEditor 4 is an easy task. Just follow these simple steps:

 1. **Download** a zipped file from kelvinthiongo's github repo:
    https://github.com/kelvinthiongo/ckeditor/archive/master.zip.
 2. **Extract** (decompress) the downloaded file into the root of your website(public directory).
 3. **Rename** the resulting folder from ckeditor-master to ckeditor.
 4. **Integrate** ckeditor by including the following sript tag:
    <script src="<yourwebsite>/ckeditor/ckeditor.js"></script>. Replace 'yourwebsite' with your website.
 5. **Associate** ckeditor to a textarea by assigning class 'ckeditor' to the textarea and you are done my fren!

**Note:** You can always change the configuration of the ckeditor in the /ckeditor/config.js.

## Checking Your Installation

The editor comes with a few sample pages that can be used to verify that
installation proceeded properly. Take a look at the `samples` directory.

To test your installation, just call the following page at your website:

	http://<your site>/<CKEditor installation path>/samples/index.html

For example:

	http://www.example.com/ckeditor/samples/index.html
