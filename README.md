# EE800

Here I use the BioID face dataset.  In order to achieve VGG lightweight face recognition classification, I chose 5 categories as examples.  

First, the original image is cut into 224×224 pictures, because the input requirements of VGG are 224×224, and 24 types of face are formed at the same time.  

The program 'format conversion' is used to convert original images to data form. Since VGG convolution computation is for pure data, images are converted to data.  

The purpose of 'Merge into Total Data Set' is to attach labels to each category.  That's the output category, 24 categories, 0 to 23.  Since we are using the 5 category as an example, our category labels are 0 to 4.  

‘vgg’is the vgg11 constructuion I used for the project.

'main1' is the program that does not reduce the number of parameters, and the classification accuracy is about 80% or more.  

'main3' this program is to replace the conventional convolution calculation process with depthwise separable convolution to achieve the reduction of parameters, the call VGG subfunction is 'vgg3'.  

After running main3 program, the classification accuracy can reach 100% after reducing parameters.


I'm still working on the final report. Thanks for your patience.
