## [Vrooboo! Wabbo!!](https://umatrix-rules.github.io/#ovagarava---toc)
### uMatrix 面板元素功能的解释

![](../assets/power.png) 当前站点下的临时开关（创建临时规则 `matrix-off: example.com true` ）。数字角标为域名计数。

![](../assets/dots.png) 一些内置隐私工具的站点开关。全局设置位于 uMatrix 控制台的 `设置` 选项卡。数字角标为当前站点已开启的工具数量。

![](../assets/lock.png) 保存全部临时规则，仅当临时规则存在时才处于可点击状态。数字角标为待提交的规则数量。

![](../assets/erase.png) 擦除全部临时规则，仅当临时规则存在时才处于可点击状态。

![](../assets/expand.png) 点击展开或折叠内置订阅拦截的域名（控制台的 `域名文件` 选项卡）。有时候这些域名并不出现在底部，例如 `pingjs.qq.com`，这种情况下，显示为 `永久规则`。

---

`红色方块（或色盲模式下的蓝色方块）`：已阻止的元素。

`绿色方块（或色盲模式下的黄色方块）`：已允许的元素。

`浅色方块`：全局规则。

对于当前站点，在以上三种类型的任一方块上，点击方块上半部分以放行对应元素；点击下半部分以拦截。

`深色方块（带小三角）`：当前站点永久规则。

- `深红色方块（或色盲模式下的深蓝色方块）`：点击上半部分以撤销，但是对应元素仍有可能被全局规则拦截。
- `深绿色方块（或色盲模式下的深黄色方块）`：点击下半部分以撤销。

`深色方块（不带小三角）`：当前站点临时规则。

### Reeshoova! - 许可协议

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a>
除非额外声明，否则本组织中全部内容许可协议均为 <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY-NC-SA 4.0 International License</a>