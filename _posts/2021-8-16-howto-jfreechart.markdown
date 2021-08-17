---
layout: post
title:  "JFreeChart乱码"
date:   2021-8-14 16:12:43 +0800
categories: HOWTO
---
在使用时发现中文环境的图表会出现乱码
对应方法：为JFreeChart设置传统主题

ChartFactory.setChartTheme(StandardChartTheme.createLegacyTheme());

在iDempiere中的createChart时，第一行就控制主题

	public JFreeChart createChart() {
		
		ChartFactory.setChartTheme(StandardChartTheme.createLegacyTheme());
		

