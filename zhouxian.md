##  配置说明

### 基础环境要求
| 组件       | 最低配置要求          |
|------------|----------------------|
| 浏览器     | Chrome 90+/Firefox 85+ |
| 分辨率     | 1280×720 及以上      |
| 网络环境   | 支持本地/在线访问     |

##  常见问题解答

### 安装相关问题

**Q1：页面打开后显示空白**  
 **解决方案**：  
1. 检查浏览器控制台报错（快捷键 `F12` > 选择"控制台"选项卡）  
2. 确认项目包含以下目录结构：  
   ```
   images/
   ├── react.png
   ├── angular.png
   ├── vue.png
   └── ...（共8个图标文件）
   ```  
3. 检查 `index.html` 中图片路径配置是否正确：  
   ```html
   <img src="images/react.png" alt="React图标">
   ```

**Q2：重置按钮点击无响应**  
 **排查步骤**：  
1. 检查浏览器是否拦截了弹窗（地址栏右侧查看）  
2. 确认 `js/script.js` 中包含以下事件监听代码：  
   ```javascript
   resetButton.addEventListener('click', initGame);
   ```

### 操作优化问题

**Q3：卡片翻转动画卡顿**  
 **优化方案**：  
```css
/* 在 css/style.css 中添加 */
.card {
  transform: translateZ(0);  /* 开启GPU加速 */
  transition: transform 0.3s ease; /* 适当调整动画时间 */
}
```

**Q4：移动端点击延迟**  
 **临时解决方案**：  
```javascript
// 在 js/script.js 中补充触摸事件
card.addEventListener('touchstart', function(e) {
  e.preventDefault();
  handleCardClick(e); 
});
```

### 逻辑处理问题

**Q5：已匹配卡片仍可点击**  
 **修正方案**：  
```javascript
// 匹配成功后应执行：
card.classList.add('matched');
card.removeEventListener('click', handleCardClick);
```

**Q6：后台标签页计时异常**  
 **根本解决方案**：  
1. 使用 Web Workers 独立运行计时器  
2. 参考实现文档：  
   ```markdown
   详见 [/docs/timer-fix.md] 中的示例代码
   ```
```
<!--by zhouxian-->