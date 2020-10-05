# Python工程目录模板

[toc]

## DL-Project-Template（深度学习工程模板）

> **[深度学习工程模板](https://github.com/SpikeKing/DL-Project-Template)**（DL Project Template），简化加载数据、构建网络、训练模型和预测样本的流程。

参考链接： [深度学习工程模板](https://juejin.im/post/6844903592764129288)

```txt
├── bases
│   ├── data_loader_base.py             - 数据加载基类
│   ├── infer_base.py                   - 预测样本（推断）基类
│   ├── model_base.py                   - 网络结构（模型）基类
│   ├── trainer_base.py                 - 训练模型基类
├── configs                             - 配置文件夹
│   └── simple_mnist_config.json
├── data_loaders                        - 数据加载文件夹
│   ├── __init__.py
│   ├── simple_mnist_dl.py
├── experiments                         - 实验数据文件夹
│   └── simple_mnist                    - 实验名称
│       ├── checkpoints                 - 存储的模型和参数
│       │   └── simple_mnist.weights.10-0.24.hdf5
│       ├── images                      - 图片
│       │   └── model.png
│       └── logs                        - 日志，如TensorBoard
│           └── events.out.tfevents.1524034653.wang
├── infers                              - 推断文件夹
│   ├── __init__.py
│   ├── simple_mnist_infer.py
├── main_test.py                        - 预测样本入口
├── main_train.py                       - 训练模型入口
├── models                              - 网络结构文件夹
│   ├── __init__.py
│   ├── simple_mnist_model.py
├── requirements.txt                    - 依赖库
├── trainers                            - 训练模型文件夹
│   ├── __init__.py
│   ├── simple_mnist_trainer.py
└── utils                               - 工具文件夹
    ├── __init__.py
    ├── config_utils.py                 - 配置工具类
    ├── np_utils.py                     - NumPy工具类
    ├── utils.py                        - 其他工具类

```

