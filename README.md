# nilm-tensorflow-env
nilm tensorflow env for base algorithm (rewrite nilm for tensorflow 2.x ,not include nilmtk package)

# 说明
1.由于tensorflow 2.x版本和新一代显卡推出后，nilmtk库已经很难适配tensorflow和最新显卡的计算了，本仓库主要记录个人在配置基于tensorflow框架的nilm环境中所遇到的问题，gan_nilm_tensorflow.yaml是环境最终配置成功的python环境。
2.nilmtk和nilmtk-contrib库不适配tensorflow 2.x，所以在本地环境中使用tensorflow重写了nilmtk和nilmtk-contrib的一些数据预处理和深度学习计算的基准算法，用于本人的论文实验对比。

# 环境硬件
1.python 3.8
2.RTX 4070
3.cuda 11.8和cuda 11.2
4.cudnn 8.9和cudnn 8.1



