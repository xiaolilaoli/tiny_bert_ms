# tiny_bert_ms
tiny_bert on mindspore

介绍了Bert与TinyBert 并在mindspore上运行。

ipynb文件可以端到端运行， 但需要提前下载好预训练模型。 在bert文件夹下，缺少由tensorflow转换来的模型。
ms2tf包含了转换的代码，具体模型下载转换操作见tinybert.ipynb的模型准备部分。

下面是路径结构

```
.tiny_bert_ms/
└── bert                                    # 模型相关文件代码。
    ├── ms2tf                                     #存放将tf的bert模型转ms模型的代码
    ├── uncased_L-12_H-768_A-12                   # 存放tf模型相关文件，包含词表和config
    └── tf2ms.ipynb                               # tf转ms的操作代码。 需要环境中存在tf和ms
    
└── config                                  # 训练设置的yaml文件。
└── data                                    # 训练所需数据
└── ipyphoto                                # ipy文件中的图片
└── tinybert.ipynb                          # 主体代码， 包含原理介绍与代码解析。


```
