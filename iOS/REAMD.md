###UIImage(fixOrientation)

http://stackoverflow.com/questions/5427656/ios-uiimagepickercontroller-result-image-orientation-after-upload 

A UIImage has a property imageOrientation, which instructs the UIImageView and other UIImage consumers to rotate the raw image data. There's a good chance that this flag is being saved to the exif data in the uploaded jpeg image, but the program you use to view it is not honoring that flag.
To rotate the UIImage to display properly when uploaded, you can use this category.