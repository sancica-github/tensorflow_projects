####MINST入门
1. Softmax常用于给不同的对象分配概率，最后一步通常情况下用softmax进行分配概率。
2. one-hot vectors 表示标记。
3. 在python语言中，tensor类型是numpy ndarry类型。
4. 使用 with tf.device(): 可指定使用哪一个gpu。
5. ×二阶张量对应于二阶矩阵，一阶张量对应于一阶矩阵，可以使用t[i,j]/t[i,j,k]访问特定的元素。
6. 
####NINIST进阶
1. 与ｃ++后端的连接叫做session．
2. tensorflow的流程是先创建一个图，然后在session中启动它。
3. 图用来计算、在session的上下文执行图、用tensor（类型化的多维数组）表示数据、用Variable维护状态、使用feed和fetch为任意的操作复制或者从中获取数据。
4. tensorflow程序通常被组织成一个图来表示和训练神经网络，有构建阶段和执行阶段。
5. estimator:代表一个完整的模型，estimator API提供方法。dataset API提供一些方法来加载和操作数据，并将数据返回到模型中。
####常见API及作用
1. tf.name_scope():主要用于管理一个图里面的各种op,方便管理参数命令，长和tf.Variable()一起使用，定义参数
2. tf.variable_scope()长结合tf.get_variable()，实现变量共享。