新闻、热点新闻

# 王木木的第一个Github项目
-
time: 2016-10-07 20:09

> ### 一、介绍

按时打卡是的哈卡萨丁**阿斯达**阿斯达打阿斯达  

1. 阿斯达
2. 阿斯达
3. 阿斯达按时
4.  阿斯达as

```Java
package test;

import java.util.List;
import java.util.Map;

import lvtao.model.Sample;
import lvtao.service.DicisionTree;

public class Main {
	public static void main(String[] args) throws Exception {

		// String[] attrNames = new String[] { "AGE", "INCOME", "STUDENT",
		// "CREDIT_RATING" };
		// 属性名称（年龄，长相，收入，公务员）
		String[] attrNames = new String[] { "AGE", "APPEARENCE", "INCOME",
				"CIVIL_SERVANT" };

		// 样本属性及其所属分类（数组中的最后一个元素为样本所属分类）
		// Object[][] rawData = new Object[][] {
		// { "<30  ", "High  ", "No ", "Fair     ", "0" },
		// { "<30  ", "High  ", "No ", "Excellent", "0" },
		// { "30-40", "High  ", "No ", "Fair     ", "1" },
		// { ">40  ", "Medium", "No ", "Fair     ", "1" },
		// { ">40  ", "Low   ", "Yes", "Fair     ", "1" },
		// { ">40  ", "Low   ", "Yes", "Excellent", "0" },
		// { "30-40", "Low   ", "Yes", "Excellent", "1" },
		// { "<30  ", "Medium", "No ", "Fair     ", "0" },
		// { "<30  ", "Low   ", "Yes", "Fair     ", "1" },
		// { ">40  ", "Medium", "Yes", "Fair     ", "1" },
		// { "<30  ", "Medium", "Yes", "Excellent", "1" },
		// { "30-40", "Medium", "No ", "Excellent", "1" },
		// { "30-40", "High  ", "Yes", "Fair     ", "1" },
		// { ">40  ", "Medium", "No ", "Excellent", "0" } };
		Object[][] rawData = new Object[][] {
				{ ">30 ", "BeautifulOrMedium", "High  ", "Yes", "0" },
				{ ">30 ", "BeautifulOrMedium", "High  ", "No ", "0" },
				{ ">30 ", "BeautifulOrMedium", "Low   ", "Yes", "0" },
				{ ">30 ", "Uglily           ", "High  ", "Yes", "0" },
				{ ">30 ", "Uglily           ", "High  ", "No ", "0" },
				{ "<=30", "BeautifulOrMedium", "High  ", "Yes", "1" },
				{ "<=30", "BeautifulOrMedium", "High  ", "No ", "1" },
				{ "<=30", "BeautifulOrMedium", "Low   ", "Yes", "0" },
				{ "<=30", "BeautifulOrMedium", "Low   ", "No ", "0" },
				{ "<=30", "BeautifulOrMedium", "Medium", "Yes", "1" },
				{ "<=30", "BeautifulOrMedium", "Medium", "No ", "0" },
				{ "<=30", "Uglily           ", "High  ", "Yes", "0" },
				{ "<=30", "Uglily           ", "High  ", "No ", "0" },
				{ "<=30", "Uglily           ", "Low   ", "Yes", "0" },
				{ "<=30", "Uglily           ", "Low   ", "No ", "0" },
				{ "<=30", "Uglily           ", "Medium", "Yes", "0" },
				{ "<=30", "Uglily           ", "Medium", "No ", "0" } };

		// 读取样本集
		Map<Object, List<Sample>> samples = DicisionTree.readSamples(attrNames,
				rawData);

		// 生成决策树
		Object decisionTree = DicisionTree.generateDecisionTree(samples,
				attrNames);

		// 输出决策树
		DicisionTree.outputDecisionTree(decisionTree, 0, null);
	}
}

```

![asda](http://images.apple.com/v/mac/home/t/images/home/macbook_opt_large_2x.jpg)

