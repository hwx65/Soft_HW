在这一部分中，我们将讨论软件工程中与漏洞报告分类有关的一些代表性工作。

漏洞报告分类是一个热门的研究领域，Antoniol等人使用ADTree、朴素贝叶斯和逻辑回归等方法对用户报告的文本进行二元分类，判断报告的内容是否为漏洞[1]。使用机器学习算法对漏洞报告进行分类可能会受到数据噪声的影响，Kim等人聚焦于缺陷数据中的噪声检测、噪声消除方法[2]。Dommati等人主要关注漏洞报告分类中的特征提取、减少数据噪声等问题，提出了一种基于朴素贝叶斯的的分类方法[3]。

除了对用户报告做二元分类以判断是否包含漏洞，一些工作还对漏洞的类型进行更细粒度的分类。Limsettho等人使用无监督的方法，通过聚类将漏洞报告自动分组，然后再自动化地为每一组生成一个代表性的名称[4]。Thung等人使用有监督学习的方法，基于SVM将漏洞分为三类，即控制和数据流（control and data flow）, 结构的 （structural）和非功能的（non-functional）[5].

Herzig等人手动检查了来自5个开源项目的7000多个漏洞报告，发现其中33.8%被错误地分类，39%被标记为有缺陷的文件其实并不包含漏洞[6]。一些被误分类的报告并不涉及对代码的修复，而与新功能、文档更新、重构等相关，这样的误分类会使易错代码定位等工作产生偏差。为了应对这一问题，Kochhar等人提出了一种基于多种特征判断漏洞报告是否需要重分类的方法，并对来源于HTTPClient, Jackrabbit, Lucene-Java, Rhino, and Tomcat5这五个开源项目的漏洞报告进行预测[7]。Xuan等人则基于朴素贝叶斯和最大期望算法提出了一种半监督的漏洞文本分类方法，以缓解人为标记的训练集中存在的误分类问题[8]。



[1]Antoniol G, Ayari K, Di Penta M, et al. Is it a bug or an enhancement? A text-based approach to classify change requests[C]//Proceedings of the 2008 conference of the center for advanced studies on collaborative research: meeting of minds. 2008: 304-318.

[2]Kim S, Zhang H, Wu R, et al. Dealing with noise in defect prediction[C]//2011 33rd International Conference on Software Engineering (ICSE). IEEE, 2011: 481-490.

[3]Dommati S J, Agrawal R, Kamath S S. Bug Classification: Feature Extraction and Comparison of Event Model using Na\" ive Bayes Approach[J]. arXiv preprint arXiv:1304.1677, 2013.

[4]Limsettho N, Hata H, Monden A, et al. Automatic unsupervised bug report categorization[C]//2014 6th International Workshop on Empirical Software Engineering in Practice. IEEE, 2014: 7-12.

[5]Thung F, Lo D, Jiang L. Automatic defect categorization[C]//2012 19th Working Conference on Reverse Engineering. IEEE, 2012: 205-214.

[6]Herzig K, Just S, Zeller A. It's not a bug, it's a feature: how misclassification impacts bug prediction[C]//2013 35th International Conference on Software Engineering (ICSE). IEEE, 2013: 392-401.

[7]Kochhar P S, Thung F, Lo D. Automatic fine-grained issue report reclassification[C]//2014 19th International Conference on Engineering of Complex Computer Systems. IEEE, 2014: 126-135.

[8]Xuan J, Jiang H, Ren Z, et al. Automatic bug triage using semi-supervised text classification[J]. arXiv preprint arXiv:1704.04769, 2017.