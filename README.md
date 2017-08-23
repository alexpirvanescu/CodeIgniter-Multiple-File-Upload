#CodeIgniter Multiple Upload Library
Just an extension to the existing Upload class to take advantage of multiple uploads in one form field

##v.0.4: August 23, 2017

__Changes__
Replacing clean_file_name() with sanitize_filename() in order to support CI3. Adding new method to get the uploaded files information.

##v.0.3: January 10, 2012

__Changes__
Adding the support of custom file names passed as an array of strings (ex image1.jpg, image2.jpg). This would help generate the filenames based on parameters like Ids of Product etc.

##v.0.2: November 7, 2011

__Changes__
Added a parameter to return all the uploaded file(s) info as opposed to boolean. Set to false to return boolean instead.

##v.0.1: July 7, 2011

__Description__
This version is a quick and dirty first pass for a project I'm currently working on. I haven't worked on the error reporting piece yet, so feel free to send in that contribution if you're so inclined.

__Installation__
Copy MY\_Upload.php to your application/libraries directory.
If you are using a prefix other than MY_ for your classes and/or alternative file paths, adjust accordingly.

__Usage__
Load the Upload class as usual, in your controller call the function `do_multi_upload()`. If you are uploading a single file, it'll default to the regular `do_upload()` method. 
In the form, set field names to array (e.g. name="userfile[]")

