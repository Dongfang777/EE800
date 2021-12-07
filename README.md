# EE800
这里我选用了BioID人脸数据集。为了实现VGG轻量化的人脸识别分类。我选择了里面的5个类别作为例子。
先将原始图像剪切成224×224大小的图片，因为VGG的输入要求是224×224的,同时形成24类人脸.
‘format conversion'这个程序的作用是将原始的图片转换成数据形式，因为VGG卷积计算是针对于纯数据，所以要把图片转换成数据。
‘Merge into total data set’的作用就是将每一类附上标签。也就是输出的类别，24类的话就是0-23。因为咱们以5分类为例，所以咱们的类别标签是0-4。
‘VGG’is the vgg11 constructuion I used for the project.
