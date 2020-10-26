# CCKS2019-IPRE任务 数据集介绍

下载方式详见：https://github.com/buppt/ChineseNRE/issues/7

或提交issues找我

## 训练集（远监督方式自动生成）
1) sent_train.txt 
```
每行是：句子ID	实体1 实体2 句子(分词后)

注：以下将一行简称为一个实例
```
2) sent_relation_train.txt
```
每行是：实例的ID 对应的关系标签ID

注：标签id和标签名的对应关系见relation2id.txt
```
3) bag_relation_train.txt
```
每行是：关系包(bag)的ID 实体1 实体2 包含该实体对的实例ID(可能多个) 关系标签ID
```
## 验证集（人工标注）
1) sent_dev.txt
```
同上，每行是：一个实例
```
2) sent_relation_dev.txt
```
同上，每行是：实例的ID 对应的关系标签ID
```
3) bag_relation_dev.txt
```
同上，每行是：关系包(bag)的ID 实体1 实体2 包含该实体对的实例ID(可能多个) 关系标签ID
```
## 测试集
1) sent_test.txt
```
同上，每行是：一个实例
```
2) sent_relation_test.txt
```
每行是：仅实例ID
```
3) bag_relation_test.txt
```
每行是：关系包(bag)的ID 实体1 实体2 包含该实体对的实例ID(可能多个) 关系标签ID
```
## 关系表
1) relation2id.txt
```
人物关系名 对应关系ID值
```
## 文本语料
1) text.txt
```
大规模无标注语料(可用于训练词向量和语言模型，例如可以交给bert做预训练)
```