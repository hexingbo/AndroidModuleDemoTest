# AndroidModuleDemo
使用组件化的一个二维码扫描Demo
### https://www.jianshu.com/p/8d0debd2c60c

#### 需求
最近公司在做一款新的车机 Launcher，需要将一个类似QQ音乐、喜马拉雅的音频模块放入其中，整体作为一个 Launcher，虽然产品一再确定，后面不会进行拆分，但是小心为上，将 Launcher 和 音频软件分为两个 App 开发，两个团队开发互不影响，最后通过组件化，作为 module 引入到空壳App中。

### 思路
这里写个组件化二维码扫描的 Demo ，①空壳 App，②公共 Library，③第一个 App 类似于上面说的 Launcher，④第二个 App 类似于上面说的音频 App。其中③、④均是可单独运行的 module，都依赖于②，当运行①时，需要将③、④转换为 library 去依赖。

## https://upload-images.jianshu.io/upload_images/7345261-0a54e74d697278c9.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/334/format/webp
