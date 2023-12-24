# Computer-Vision-OpenCV-Basics

# Basic Operations

#### imread
#### https://www.geeksforgeeks.org/python-opencv-cv2-imread-method/
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/022f1b4c-6d28-4e99-a5f9-0fc8f7d472a3)

#### VideoCapture
#### https://www.geeksforgeeks.org/python-opencv-capture-video-from-camera/
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/85e4f51e-8c32-40be-8ebb-08786189fada)

#### copyMakeBorder
#### https://www.geeksforgeeks.org/python-opencv-cv2-copymakeborder-method/
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/70607f60-952d-4acf-a9f1-ee1f188d1cd1)

#### resize
#### https://www.geeksforgeeks.org/image-resizing-using-opencv-python/

#### cvtColor
#### https://www.geeksforgeeks.org/python-opencv-cv2-cvtcolor-method/
#### https://docs.opencv.org/4.x/df/d9d/tutorial_py_colorspaces.html
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/f2f2b428-d2c6-422b-bd00-92b36899ba6f)

# Threshold and Blur
#### threshold
#### https://www.geeksforgeeks.org/python-thresholding-techniques-using-opencv-set-1-simple-thresholding/
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/507239a1-4173-4f8c-83d2-503610ff81e2)

#### Blur
#### https://docs.opencv.org/4.x/d4/d13/tutorial_py_filtering.html
#### https://www.geeksforgeeks.org/opencv-python-program-to-blur-an-image/
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/fb2d6f92-cf48-4d2a-b13c-993f065a4da4)

#### Gaussian Blur
#### https://docs.opencv.org/4.x/d4/d86/group__imgproc__filter.html#gaabe8c836e97159a9193fb0b11ac52cf1
#### https://blog.csdn.net/farmwang/article/details/74452750
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/f1b4151c-4ad4-422d-a1fa-a06dc2ce18a3)
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/a7bc6a04-bbe2-4a88-80d8-87d718bf8966)

#### How to get the Gaussian kernel: 
#### larger sigma = smaller middle pixel contribution, larger neighbor contribution, more blur
#### smaller sigma = larger middle pixel contribution, smaller neighbor contribution, less blur
#### large kernel size = more blur
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/7b7c9e3f-5e7e-41c9-af70-3cb2ac029fdc)
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/62fc88ff-7665-4559-bf01-f4e5c3ab34ef)

#### Morphological Transformations
#### Erode & Dilation
#### https://docs.opencv.org/3.4/db/df6/tutorial_erosion_dilatation.html
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/a5f5bd31-8ab5-40bf-be23-8b4519ec1822)
![Screen Shot 2023-12-23 at 4 35 11 PM](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/b7b8202a-0d45-4f00-82cb-0f0b2bf2e7c2)
![Screen Shot 2023-12-23 at 4 35 34 PM](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/1bea1371-b935-4700-8568-750c725d7570)
![Screen Shot 2023-12-23 at 4 35 52 PM](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/5e3b3973-7264-444a-a7ad-8c3ba5e16325)


#### Morphological Transformations
#### https://docs.opencv.org/4.x/d9/d61/tutorial_py_morphological_ops.html
#### https://www.geeksforgeeks.org/python-opencv-morphological-operations/

#### Opening,  Erode -> Dilation:
![Screen Shot 2023-12-23 at 4 36 46 PM](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/8b87944e-0775-4a8e-90b9-802981116ea3)

#### Closing,  Dilation -> Erode:
![Screen Shot 2023-12-23 at 4 37 13 PM](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/15b2d4d8-8aca-4f0b-a47b-146388f4969d)

#### Top Hat,  Input - Opening
#### Src  -  Dilation( Erode( Src,Kernel ) , Kernel )
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/ad0eebf5-5ef7-49da-a2e0-ab8410fc925a)

#### Black Hat, Closing - Input

#### Erode( Dilation( Src,Kernel ) , Kernel ) - Src
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/967aab13-25ea-4e37-b1cb-941993d82060)

# Image Gradient
#### Discrete Calculus
#### https://en.wikipedia.org/wiki/Discrete_calculus![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/b8ad26e0-cc2d-4dbb-8b0a-1d5bdf897c18)
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/9cab83b3-dfde-4b93-8c23-377e4f63637a)

#### Image Gradient is used to extract information from an image and detect its edge
#### gx, the image intensity changing from left to right
#### gy, the image intensity changing from top to bottom
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/b2658a3c-5fd1-49e6-8237-ea67f4e79ce1)
#### In the discrete case, we can only take differences at one pixel intervals .
#### To avoid shifting the image by half a pixel, we select 2 pixel intervals.
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/3bd9fd88-f25b-4abf-b8cc-bb63aa447ccd)
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/39fa5f02-67f2-44b8-964a-1fbcabb56dc4)

#### Gradient Magnitude:
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/75cb0156-593f-4c38-a29e-94e9fc75b027)
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/23cce259-c0ac-4368-a94c-e5dae88b42b6)

#### Gradient Direction:
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/c2aa0f55-1564-48f3-a86f-8b1fbfe4afb1)
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/816e820e-3efe-4abb-81d0-d7873a25e5e2)

#### Image Gradient: Sobel Filter
#### https://automaticaddison.com/how-the-sobel-operator-works/
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/cb445c42-a533-4d71-b407-57a21068dec2)
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/29802ba5-ea90-45c9-b00c-eec763e533e2)
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/f64cab52-4111-4ebf-affa-36bb88d69009)

#### P5X / P5Y = P5's gradient towards x and y direction
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/0b3658df-474d-4c32-90d6-c8a40b85aa30)
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/63305cf1-e477-4112-b4be-8afc676acc56)


#### Image Gradient:  Sobel (first derivative),  Scharr (first derivative), Laplacian (second derivative)
#### https://docs.opencv.org/3.4/d2/d2c/tutorial_sobel_derivatives.html
#### https://www.projectpro.io/recipes/what-are-sobel-and-scharr-derivatives-opencv

#### Laplacian
#### https://docs.opencv.org/4.x/d5/d0f/tutorial_py_gradients.html
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/5e3386ee-0ab2-4987-b328-a5e4657cdb6b)

#### ConvertScaleAbs
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/dfc5cf7f-539b-4006-93ed-282d4f2370d5)

#### Color to Gray
https://www.dynamsoft.com/blog/insights/image-processing/image-processing-101-color-space-conversion/
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/8d85b279-98ee-4ab2-8ac5-28ec95ad4e02)
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/967c424d-26c8-4e44-8e68-dabc085f92d8)

#### Angle of Π
#### https://jarnowouda.com/what-are-radians/
![image](https://github.com/yinanericxue/Computer-Vision-OpenCV-Basics/assets/102645083/ab2727f7-90ff-4712-a540-3e095bd34ed5)
