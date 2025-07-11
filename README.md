# 📖 TextClarity 清晰文本助手  
## ✨ 让网页文字告别发虚！ 
### 🔗 其他链接  
- 脚本源码：[GitHub 仓库](https://github.com/521-baby/ChaoXing-SuperSrarLearn)    
- 如果有帮助到你<img src='https://github.com/521-baby/ChaoXing-SuperSrarLearn/blob/main/%E5%AD%A6%E4%B9%A0%E9%80%9A%E8%84%9A%E6%9C%AC.js' width='16px' /> 投喂渠道：[⚡爱发电](https://afdian.com/a/chunshu) or [微信赞赏](https://github.com/521-baby/521-baby/blob/main/DONATE.md) or [支付宝](https://github.com/521-baby/521-baby/blob/main/DONATE2.md)</del>
### 访客人数：
<img src="https://count.kjchmc.cn/get/@TextClarity-Assistant?theme=asoul" alt="如果您无法看到此内容，请刷新页面。">  

Windows浏览器常遇文字模糊、颜色淡的问题，本脚本通过调节文字描边强度，让内容更清晰易读，支持Chrome/Edge/Firefox等主流浏览器～  

### 🌟 核心功能  
- **🔍 清晰度自由调节**：0-1.0强度滑块，实时预览文字锐利度变化  
- **🌐 网站白名单管理**：右键一键屏蔽特定网站效果，避免过度增强  
- **🎛 便捷设置面板**：基于SweetAlert2的可视化界面，操作直观  

### 🚀 快速开始  
#### 1. 安装准备  
- 先安装脚本管理器：    
[Tampermonkey](https://tampermonkey.net/)（Chrome/Edge）或    
[Greasemonkey](https://addons.mozilla.org/firefox/addon/greasemonkey/)（Firefox）  
#### 2. 安装脚本  
- 点击下方链接一键安装：  
  [📥 安装 📖 TextClarity 清晰文本助手 油猴脚本](https://greasyfork.org/zh-CN/scripts/539737-textclarity%E6%B8%85%E6%99%B0%E6%96%87%E6%9C%AC%E5%8A%A9%E6%89%8B)
  
  [📥 安装 📖 TextClarity 清晰文本助手 脚本猫脚本](https://scriptcat.org/zh-CN/script-show-page/3638)
- 浏览器会自动跳转至安装页面，点击 **安装** 即可完成

### 🎮 使用指南  
![屏幕截图 2025-06-17 234945.png](https://scriptcat.org/api/v2/resource/image/xzZAdDLWcacdWer5)
#### ▶ 首次设置  
1. 安装后首次访问网页会自动弹出设置面板  
2. 拖动滑块（0为原始状态，1为最强）观察文字变化  
3. 点击"保存"应用设置，或"还原"重置  

#### ▶ 日常操作  
- **调整清晰度**：    
右键网页空白处 → ⚙ 设置 → 拖动滑块实时生效  
- **白名单管理**：    
进入目标网站 → 右键 → 💡 当前网站：✔（添加白名单）    
白名单网站会显示为💡 当前网站：❌，点击可取消屏蔽  

### ⚙ 技术原理  
通过CSS的`text-stroke`属性为文字添加轮廓：  
```css
*:not(pre) {    
-webkit-text-stroke: ${val}px; /* Chrome/Edge */    
text-stroke: ${val}px;         /* Firefox */
}
```  
- 排除`<pre>`标签（代码块），避免影响代码格式  
- 选中文字时背景色设为`#338fff`，提升可读性  

### 📊 兼容性表  
| 浏览器        | 支持状态 | 备注                  |  
|---------------|----------|-----------------------|  
| Chrome        | ✅ 完美   | 50+版本               |  
| Firefox       | ✅ 完美   | 需启用实验特性        |  
| Edge          | ✅ 完美   | Chromium内核版        |  
| 360/QQ浏览器  | ✅ 完美   | 极速模式下            |  
| Safari        | ⚠ 有限   | 高版本支持较好        |  

### ❓ 常见问题  
#### Q: 文字太粗/模糊怎么办？  
A: 建议将强度值调至0.1-0.3（默认0.05），高分辨率屏幕可适当提高，低分辨率建议降低。  
#### Q: 部分网站无效果？  
A: 可能原因：  
1. 网站已加入白名单（检查右键菜单状态）  
2. 网站使用Canvas渲染文字（脚本无法修改）  

### 📝 更新日志  
#### v1.0.0 (2025-06-17)  
- 初始版本发布，实现基础文字增强功能  
- 集成白名单系统和可视化设置界面  
- 兼容主流浏览器的文字描边方案  
### 📄 许可证  
MIT License © 2025 伏黑甚而  

> 💡 提示：若文字效果影响阅读体验，可随时通过右键菜单还原设置～
