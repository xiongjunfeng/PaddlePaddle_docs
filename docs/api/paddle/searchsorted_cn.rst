.. _cn_api_tensor_searchsorted:

searchsorted
-------------------------------

.. py:function:: paddle.searchsorted(sorted_sequence, values, out_int32=False, right=False, name=None)

根据给定的 ``values`` 在 ``sorted_sequence`` 的最后一个维度查找合适的索引。

参数
::::::::
    - **sorted_sequence** (Tensor) - 输入的N维或一维Tensor，支持的数据类型：float32、float64、int32、int64。该Tensor的数值在其最后一个维度递增。
    - **values** (Tensor) - 输入的N维Tensor，支持的数据类型：float32、float64、int32、int64。
    - **out_int32** (bool，可选) - 输出的数据类型支持int32、int64。默认值为False，表示默认的输出数据类型为int64。
    - **right** (bool，可选) - 根据给定 ``values`` 在 ``sorted_sequence`` 查找对应的上边界或下边界。默认值为False，表示在 ``sorted_sequence`` 的查找给定 ``values`` 的下边界。
    - **name** (str，可选) - 具体用法请参见 :ref:`api_guide_Name`，一般无需设置，默认值为 None。

返回
::::::::
Tensor(与 ``values`` 维度相同)，如果参数 ``out_int32`` 为False，则返回数据类型为int32的Tensor，否则将返回int64的Tensor。




代码示例
::::::::

COPY-FROM: paddle.searchsorted