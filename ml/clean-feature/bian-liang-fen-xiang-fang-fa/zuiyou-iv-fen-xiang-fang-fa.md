最优IV分箱方法也是自顶向下的分箱方式，期目标函数为Information Value值。IV值的计算是在WOE值的基础上演化而来的。

![](https://pic1.zhimg.com/80/v2-5e4c2ff07805edd25195fa92f9a626ec_720w.webp)

其中M为分组的个数，本例中为自顶向下的分箱方式采用的二叉树的方式，因此M=2。Goodi和Badi分别为以不同切分点划分后第i组内好坏样本的个数，Goodtotal和Badtotal为总体样本中好坏样本的个数。

IV值本质是对陈华的K-L距离，即在切分点处分裂得到的两部分数据中，选择好坏样本的分布差异最大点作为最优切分点。分箱结束后，计算每个箱内的IV值加和得到变量的IV值，可以用来刻画变量对目标值的预测能力。即变量的IV值越大，则对目标变量的区分能力越强，因此IV只还可以用来做变量选择。
