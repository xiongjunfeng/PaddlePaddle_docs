.. _cn_api_nn_ThresholdedReLU:

ThresholdedReLU
-------------------------------
.. py:class:: paddle.nn.ThresholdedReLU(threshold=1.0, name=None)

Thresholded ReLU激活层

.. math::

    ThresholdedReLU(x) = \begin{cases}
                          x, \text{if } x > threshold \\
                          0, \text{otherwise}
                         \end{cases}

其中，:math:`x` 为输入的 Tensor

参数
::::::::::
    - threshold (float，可选) - ThresholdedReLU激活计算公式中的threshold值。默认值为1.0。
    - **name** (str，可选) - 具体用法请参见 :ref:`api_guide_Name`，一般无需设置，默认值为 None。

形状：
::::::::::
    - input：任意形状的Tensor。
    - output：和input具有相同形状的Tensor。

代码示例
:::::::::

COPY-FROM: paddle.nn.ThresholdedReLU