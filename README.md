# Context-Aware-Text-Placement-on-Images-Using-Deep-Learning

Overview

This project provides a tool for adding text to images with fully customizable font, size, color, and position. The unique feature is that when text overlaps an object in the image, the text intelligently appears behind the object, creating a visually seamless result. This is achieved using deep learning for image segmentation, along with image manipulation libraries for rendering the text.
Features

1. Customizable Text: Add text with any font, size, color, and at any location.
2. Object-Aware Placement: If the text overlaps with an object, it is placed behind the object.
3. Accurate Segmentation: Uses state-of-the-art DeepLabV3 with ResNet-50 for precise object segmentation.
4. Flexible Integration: Built with PyTorch, OpenCV2, and PIL, making it adaptable for various image processing tasks.

How It Works

1. Image Segmentation:
        The image is passed through a pre-trained DeepLabV3 model with a ResNet-50 backbone to segment objects and generate a pixel-wise mask         of the objects in the image.
2. Text Placement:
        The user specifies the text content, font, size, color, and location.
        If the text overlaps with an object in the image, the object mask is used to place the text behind the object.
3. Text Rendering:
        Using OpenCV2 and PIL, the text is rendered on the image, either in front of or behind objects based on the segmentation output.

Technologies Used

* DeepLabV3 with ResNet-50: For image segmentation to identify objects in the image.
* PyTorch: For running the deep learning model.
* OpenCV2: For image processing.
* PIL (Python Imaging Library): For rendering and manipulating images.

Sample OutPuts:
![Screenshot from 2024-10-15 18-43-34](https://github.com/user-attachments/assets/737b9c4d-2794-473b-8bb2-a91fe3b2d54f)
![Screenshot from 2024-10-15 18-43-23](https://github.com/user-attachments/assets/24ad4956-7177-41c8-955d-6eee0e84c519)

