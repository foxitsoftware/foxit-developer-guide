## 如何删除相机图标？(iOS, complete_pdf_viewer)

RDK提供的demo complete_pdf_viewer中，初始界面的右下角有个相机图标，这实际上是Scan功能按钮。


仅移除相机图标
在demo代码里做调整：

\complete_pdf_viewer\Source\ViewController.m
self.openScanBtn.hidden确保设置为YES
或者将 openScanBtn及相关代码都去掉。
 

去掉Scan功能
如果还想将Scan功能里彻底移除的话：

包中/docs下的developer guide文档里，有教如何将加入Scan功能：

” 3.1.2 Integrate Foxit PDF SDK for iOS into your apps“和” 3.1.6 Add the scanning feature based on the full-featured PDF Reader“
或者
“ 3.2.2 Integrate Foxit PDF SDK for iOS into your apps”和“ 3.2.6 Add the scanning feature based on the full-featured PDF Reader”

可以参考这部分说明，并将相关的库和代码都去掉，就能从complete_pdf_viewer里去掉Scan功能了。
