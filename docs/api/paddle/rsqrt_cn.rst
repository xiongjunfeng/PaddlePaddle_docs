.. _cn_api_fluid_layers_rsqrt:

rsqrt
-------------------------------

.. py:function:: paddle.rsqrt(x, name=None)




rsqrt激活函数。

注：输入x应确保为非 **0** 值，否则程序会抛异常退出。

其运算公式如下：

.. math::
    out = \frac{1}{\sqrt{x}}


参数
::::::::::::

    - **x** (Tensor) – 输入是多维Tensor，数据类型可以是float32和float64。 
    - **name** (str，可选) - 具体用法请参见 :ref:`api_guide_Name`，一般无需设置，默认值为 None。

返回
::::::::::::
Tensor，对输入x进行rsqrt激活函数计算结果，数据shape、类型和输入x的shape、类型一致。

代码示例
::::::::::::

COPY-FROM: paddle.rsqrt