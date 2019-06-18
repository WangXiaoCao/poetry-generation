## AI诗歌创作
利用RNN生成古诗词序列、歌词、现代诗、散文。
无论生成何种模式的文字，其本质都是基于字或基于词的序列生成。

## 数据源
古诗词数据来自于https://github.com/chinese-poetry/chinese-poetry， 这里有整理好的规模较大的唐诗宋词元曲诗经等等，可clone该项目有效利用其中数据

## 项目结构
- 核心代码
    - config.py  配置文件
    - dataHandler.py 数据预处理
    - model.py  模型
    - train.py  训练模型
    - samples.py  采样诗歌
- 文件夹
    - data 存放预处理好的数据文件：char_dict, car_to_ix, ix_to_char
    - model 存放保存的模型

## 如何使用
### 1.修改配置
在训练模型之前，打开config.py文件，对一些参数进行自定义的修改，比如模型与数据的路径、模型的超参数、生成序列的长度等等。


### 2.训练
运行train.py文件
```
python train.py
```


### 3.预测
运行sample.py文件
```
python sample.py
```





