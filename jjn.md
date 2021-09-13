 <center>
     <h1>姜佳男-13161322066-高级算法工程师</h1>
 </center>

## 个人信息 

* 性 别：男&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;年 龄：29  
* 手 机：13161322066 &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;  邮 箱：jiangjianan037@126.com    
* 专 业：自动化 &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;岗 位：高级算法工程师

## 工作及教育经历


* 嘀嘀&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&ensp;2019.8~至今&emsp;&emsp;&emsp;&emsp;&emsp; Voyager-Autonomy       
* 北京邮电大学&emsp;&emsp;&emsp;&emsp;&emsp;2016.9~2019.7&emsp;&emsp;&emsp;&emsp; 自动化-研究生         
* 青岛理工大学&emsp;&emsp;&emsp;&emsp;&emsp;2011.9~2015.7&emsp;&emsp;&emsp;&emsp; 自动化-本科  


## 项目经历

1. Voyager - V2X 检测追踪算法开发与部署 - 独立开发 - 2020/11 - 至今 
    * 具体功能：高点相机目标检测与追踪，输出目标位置信息，配合车端感知
    * 技术方案：使用YOLOV5开发目标检测算法，DeepSORT作为目标追踪算法，在服务器上使用Pytorch训练YOLOV5模型，并使用Tensorrt框架在Xavier上部署检测与追踪算法。使用YOLOX更新目标检测算法。
    * 项目难点与解决方案：
        * 数据集类别不平衡：引入AP Loss，改善数据类别不平衡带来的问题
        * 部分类别错检、误检严重：1. 修改DeepSORT追踪器，使当前帧的分类与之前帧匹配的目标分类结果结合，在不增加计算量
的同时减缓误检问题 2. 误检图片作为background图片加入训练
        * 原开发框架用pytorch，修改模型后需要同时修改tensorrt代码线上部署代码，开发不够灵活：构建pytorch-onnx-tensorrt代码，训练模型修改后不需要重构tensorrt代码
        * 成果：算法满足服务性能要求，并部署到线上
2. Voyager - 鱼眼相机标定 - 独立负责 - 202103- 202106
    * 具体功能：对不同型号鱼眼相机进行内参与外参标定
    * 技术方案：采集部分相机标定板图片，使用Mei模型标定相机内参，对缺失标定板图片的相机使用同批次相机标定板图片进行标定
    * 项目难点与解决方案：
        *  线上测试标定算法速度过慢：使用opencv cuda接口重写算法代码
    * 成果：1. 相机目标检测与追踪算法已部署到端上所有点位  2. 鱼眼相机内参数小于5pixel error，满足需求 
3. AI-Lab - CD-FSL竞赛 - 合作 - 2020/07-2020/10
    * CVPR Cross-Domain Few-Shot Learning竞赛第一名
    * 挑战：
        * 只使用miniImageNet数据集进行预学习
        * 只能使用极少的目标域数据训练(5张)
        * 4个目标域数据分布跨度极大
    * 个人工作：
        * 前期调研
        * 提出并实现transductive和instance classification相结合的方法
        * 撰写《A Transductive Multi-Head Model for Cross Domain Few-Shot Learning》- (https://arxiv.org/abs/2006.11384)

4. AI-Lab - 论文 - 合作 - 2020/10-2020/12
    * 《Multi-view Correlation based Black-box Adversarial Attack for 3D Object Detection》- KDD2021(https://doi.org/10.1145/3447548.3467432)
    * contribution：
        * 第一个基于camera和lidia传感器的3D目标检测
对抗攻击工作
        * 提出多个融合images和point cloud的生成器用
于生成攻击样本
        * 在KITTI 3D目标检测数据集上进行大量实验，并证明我们的方法性能要远远超过单支
(images攻击或point cloud攻击)方法
    * 个人工作：负责idea代码实现，论文画图，可视化相关工作
5. AI-Lab - 网约车新用户打车预测 - 单独负责 - 2020/04 - 2020/07
    * 项目需求：
        * 使用有完整特征的活跃用户作为源域 
        * 使用不完整特征新用户数据作为目标域 
        * 创建迁移学习模型预测新用户在未来七天使用网约车服务的概率
    * 技术方案：提出IDIAN算法
    * 项目难点与解决方案：
        * 源域与目标域数据特征空间不同：1.分别构建特征生成器对齐特征维度与空间 2.构建自编码机减少特征损失
        * 目标域数据缺失与源域域间差异大：1.使用缺失mask与随机噪声设置预估生成器生成特征缺失部分的预估值 2.使用Adversarial Domain Adaptation对齐源域与目标域的特征
    * 项目成果： 
        * 预测准确率超过目前已经公开的模型，F1 score较基准提高3.8%。
        * 撰写论文《Domain Adaptation with Incomplete Target Domain》- (https://arxiv.org/abs/2012.01606)
6. 营业执照目标检测与识别 - 实习 -2018
    * 使用Faster RCNN 检测营业执照字段，并使用CRNN识别字段内容
7. 钢轨扣件检测 - 学校项目 - 2017
    * 使用 Faster RCNN检测钢轨扣件
8. 微信公众号爬虫 - 2016
    * 客户输入关键字，使用python爬取微信公众号相关内容，并使用使用Django可视化展示，并用Booststrap美化前端。



## 专业技能

* 熟悉Python、C++等编程语言
* 掌握基础数据结构和算法的基本原理
* 熟悉迁移学习领域和小样本学习领域基础算法
* 熟悉ResNet、VGG等主流分类模型，熟悉YOLO、FasterRCNN等检测模型


## 其他信息 
* 喜欢骑车 等等
* 性格开朗 等等 



