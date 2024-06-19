# AI-fundamental-project-2
第一步：下载项目并安装一些必要的库，如pandas、opencv-python、torch等。

第二步：下载数据集，地址如下：

https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data

首先点击Data，选择Download All（需要先注册账号获取查看数据集权限），将train.csv文件放入dataset文件夹中。

第三步：运行data_separation.py，在dataset文件夹中生成两个新的文件emotion.csv和pixels.csv。

第四步：运行data_view.py，在face_images文件夹中存有大量人脸图片。

第五步：取28709张图片中的前24000张作为训练集，其余图片作为验证集，新建两个文件夹train_set和verify_set，将0.jpg~23999.jpg放入train_set,其余图片放入verify_set，运行image_emotion_mapping.py，在train_set和verify_set文件夹中各生成一个名为image-emotion.csv的关系映射表。

第六步：运行model_CNN.py训练模型（此过程需要时间较长，cpu运行需要至少几个小时，可选择运行model_CNN_GPU.py用gpu运行可能更快），训练完成后模型文件位于model文件夹中，运行model_CNN_test.py查看最终效果。
