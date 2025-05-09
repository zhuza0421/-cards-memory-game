##  系统配置指南

### 基础运行环境要求
| 组件类别 | 详细配置要求 | 备注说明 |
|---------|------------|---------|
| 浏览器支持 | Chrome 90+ / Firefox 85+ / Edge 95+ | 推荐使用最新稳定版 |
| 显示分辨率 | 最低1280×720 | 最佳显示效果1920×1080 |
| 网络环境 | 本地访问或在线部署 | 需保证资源加载速度 |

##  常见问题解决方案

### 一、安装部署类问题

问题1：页面加载后显示空白
 完整排查方案：

1. 浏览器控制台检查（Windows按F12，Mac按Option+Command+I）
2. 资源文件完整性验证：
   - 确认项目目录存在images/资源文件夹
   - 检查必须包含的8个框架图标文件：
     ├── react.png    （React框架标识）
     ├── angular.png （Angular框架标识）
     ├── vue.png      （Vue框架标识）
     ...（其他5个配套图标）
3. 路径配置检查：
   - 确认index.html中资源引用路径正确
   - 示例：<img src="images/react.png" alt="React标志">

问题2：重置功能按钮失效
 系统化排查流程：

1. 浏览器设置检查：
   - 解除弹窗拦截设置
   - 清除浏览器缓存（Ctrl+Shift+Del）
2. 事件绑定验证：
   - 检查js/script.js文件
   - 确认存在标准事件监听代码：
     resetButton.addEventListener('click', initGame);
3. 兼容性测试：
   - 在不同浏览器环境测试功能响应

### 二、运行操作类问题

问题3：卡牌动画性能优化
 专业优化建议：

1. 硬件加速方案：
```css
    .card {
    transform: translateZ(0);
    will-change: transform;
    }
```
2. 动画参数调优：
   - 调整transition-duration至0.3s
   - 使用cubic-bezier优化运动曲线
3. 渲染性能检测：
   - 使用Chrome DevTools的Performance面板分析

问题4：移动端触控延迟
 全平台适配方案：

1. 基础事件增强：
```javascript
    card.addEventListener('touchstart', function(e) {
    e.preventDefault();
    handleCardClick(e);
    }, {passive: false});
```
2. 高级优化方案：
   - 引入FastClick库消除300ms延迟
   - 添加touch-action样式声明

### 三、逻辑功能类问题

问题5：卡牌匹配状态异常
 完整解决方案：

1. 状态管理强化：
```javascript
// 匹配成功处理逻辑
function handleMatch() {
  matchedCards.forEach(card => {
    card.classList.add('matched');
    card.removeEventListener('click', handleCardClick);
    card.style.pointerEvents = 'none';
  });
}
```
2. 防御性编程：
   - 添加状态校验逻辑
   - 增加匹配成功动画反馈

问题6：后台计时精度问题
 企业级解决方案：

1. Web Workers实现方案：
   - 创建专用计时线程
   - 实现前后台精准时间同步
2. 降级处理策略：
```javascript
// 文档参见 docs/timer-fix.md
const timerWorker = new Worker('js/timer-worker.js');
timerWorker.postMessage({action: 'start'});
```
3. 性能平衡建议：
   - 设置合理的计时频率
   - 添加节能模式切换


<!--by zhouxian-->
