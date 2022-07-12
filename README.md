# RCCapsNet
Fashion Image Retrieval With Capsule Networks

An Unofficial Notebook for https://openaccess.thecvf.com/content_ICCVW_2019/papers/CVFAD/Kinli_Fashion_Image_Retrieval_with_Capsule_Networks_ICCVW_2019_paper.pdf

based on Official code https://github.com/birdortyedi/image-retrieval-with-capsules

Deep Fashion-inshop Dataset: https://drive.google.com/drive/folders/0B7EVK8r0v71pVDZFQXRsMDZCX1E?resourcekey=0-4R4v6zl4CWhHTsUGOsTstw

contacts mahdiye_khatami@semnan.ac.ir or m.khatami95@gmail.com

![myimage-alt-tag](https://i.postimg.cc/FRtGbDyH/2022-07-09-15-58-38-Window.png)


## New changes to the original code

1. Added "Download Dataset" section
2. Added "Install Packages" section 
2. In "Config" this configs changed: **epochs = 1**, **multi_gpu=None**, **model_type='rc'**
3. In "Config" This line Changed: "args = parser.parse_args()" changed to "args, unknown = parser.parse_known_args()"
3.  In "Main/Train" this line changed:
"if i % 5 == 0: test(model=eval_model, args=args)" changed to "i % 1 == 0: test(model=eval_model, args=args)"
6. Added "eval_partioner_by_group(group)" and you can choose "group" in config.by default group='ALL'.you can ghange it to 'WOMEN' or 'MEN' and then edit the 'num_class' value.
