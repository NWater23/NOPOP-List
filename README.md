# No Popup List

这是我自己的广告拦截规则列表, 主要是一些通杀规则, 用于强力去除其它规则没有覆盖到的垃圾广告.

有可能存在误杀情况, 如有请issue报告.

仅考虑兼容uBlock Origin.

本仓库提供两个规则:

- 常规拦截 https://github.com/NWater23/NOPOP-List/raw/main/nopop-list.txt
- 强力拦截 https://github.com/NWater23/NOPOP-List/raw/main/nopop-list-force.txt

如果需要强力拦截, 请同时加载两个规则.  
强力拦截的好处是可以防止绝大多数意外打开不良网站的情况, 缺点是存在误杀.

与其它拦截规则搭配使用, 效果更好:

- Easy List
  - https://github.com/easylist/easylistchina/raw/master/easylistchina.txt
- 乘风
  - https://github.com/xinggsf/Adblock-Plus-Rule/raw/master/rule.txt
  - https://github.com/xinggsf/Adblock-Plus-Rule/raw/master/mv.txt
- Quark List
  - https://github.com/bamf2077/quarklist/raw/master/dist/quarklist.txt
- CJX's Annoyance List
  - https://raw.githubusercontent.com/cjx82630/cjxlist/master/cjx-annoyance.txt
  - https://raw.githubusercontent.com/cjx82630/cjxlist/master/cjx-ublock.txt

## 编写规则技巧

首先打开调试器, 暂停页面上所有JS脚本的运行.

注意观察这个广告是什么时候触发的, 被什么操作触发的, 反推它的触发机制.

思考广告需要的展示效果和推广目的, 从这些特征下手编写拦截规则, 这样即使它未来有了新变化, 仍然可以用原来写好的规则干掉.
