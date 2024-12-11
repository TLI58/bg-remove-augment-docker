# Background Removal with Deep Learning

This repository shows the code to remove the background of the pictures using the [U2Net](https://arxiv.org/pdf/2005.09007.pdf) pre-trained model.

The application has three simple functions:

1. Remove the background, producing a transparent PNG file.

2. Change the background by another picture.

3. Combine the image and multiple backgrounds to augment the dataset.


### Demos
![Demo](assets/demo1.gif)
<hr>

![Demo](assets/demo2.gif)

### Install

1. Download the Dockerfile
2. In the same directory run "docker build -t bg-remove ."
3. Start the Image via  "docker run -p 8000:8000 bg-remove" for example.

It schould now be reachable via 

| http://localhost:8000/ |  Front-end to perform background remove.

| http://localhost:8000/augmentation |  Front-end to perform augment images.


### References
U2Net: [https://github.com/xuebinqin/U-2-Net](https://github.com/xuebinqin/U-2-Net)


### BibTeX
    @InProceedings{Qin_2020_PR,
        title = {U2-Net: Going Deeper with Nested U-Structure for Salient Object Detection},
        author = {Qin, Xuebin and Zhang, Zichen and Huang, Chenyang and Dehghan, Masood and Zaiane, Osmar and Jagersand, Martin},
        journal = {Pattern Recognition},
        volume = {106},
        pages = {107404},
        year = {2020}
}
