
```markdown
# Technical Documentation Enhancement Request

## 1. Request for AI Markdown Format Specification
- **Purpose**: Clarify the standard Markdown format used by AI systems
- **Requirements**:
  - Detailed syntax specifications
  - Supported extensions (tables, code blocks, etc.)
  - Formatting best practices
- **Expected Output**: 
  ```markdown
  # AI Markdown Format Standard
  ## Heading Styles
  - Use ATX-style headers (#, ##)
  - Maintain consistent header hierarchy
  
  ## Code Blocks
  ```language
  // Specify language for syntax highlighting
  const example = "properly formatted";
  ```
  ```

## 2. Professional Terminology Review by AI
- **Scope**: Technical audit of five key web development terms
- **Review Criteria**:
  - Ac```markdown
# Web 前端开发核心术语

## 1. `querySelectorAll`
- **中文**：DOM 元素选择方法  
- **英文**：A DOM method that selects all elements matching a specified CSS selector and returns a static NodeList.  
- **详细说明**：  
  - 通过 CSS 选择器获取文档中所有匹配的元素
  - 返回的是静态的 `NodeList` 集合（不会随 DOM 变化自动更新）
  - 性能低于 `getElementById` 等单一选择器
- **示例**：
  ```javascript
  // 选择所有类名为 btn 的元素
  const buttons = document.querySelectorAll('.btn');
  
  // 转换为数组操作
  const buttonArray = Array.from(buttons);
  ```

## 2. `classList`
- **中文**：HTML 元素类名操作接口  
- **英文**：An interface for manipulating the class attributes of an HTML element.  
- **方法说明**：
  | 方法        | 描述                  | 示例                     |
  |------------|----------------------|-------------------------|
  | `add()`    | 添加一个或多个类名      | `el.classList.add('active')` |
  | `remove()` | 移除指定类名           | `el.classList.remove('old')` |
  | `toggle()` | 切换类名状态           | `el.classList.toggle('active')` |
  | `contains()`| 检查类名是否存在       | `el.classList.contains('active')` |
- **最佳实践**：
  ```javascript
  // 链式操作
  element.classList.add('new').remove('old');
  ```

## 3. `addEventListener`
- **中文**：事件监听方法  
- **英文**：A method to attach an event handler to an element.  
- **核心特性**：
  - 支持所有 DOM 事件类型（`click`, `scroll`, `input` 等）
  - 第三个参数可配置事件捕获/冒泡
  - 相同监听器不会重复添加
- **示例**：
  ```javascript
  // 推荐使用具名函数以便移除
  function handleClick() {
    console.log('Clicked');
  }
  
  button.addEventListener('click', handleClick);
  button.removeEventListener('click', handleClick);
  
  // 高级配置
  element.addEventListener('scroll', handler, {
    passive: true,  // 提升滚动性能
    once: true      // 只执行一次
  });
  ```

## 4. `setTimeout`
- **中文**：异步定时器函数  
- **英文**：A function that executes a callback after a specified delay.  
- **关键点**：
  - 最小延迟为 4ms（浏览器规范）
  - 返回定时器 ID（数字类型）
  - 回调函数中的 `this` 默认指向全局对象
- **示例**：
  ```javascript
  // 基本用法
  const timerId = setTimeout(() => {
    console.log('Executed after 1s');
  }, 1000);
  
  // 清除定时器
  clearTimeout(timerId);
  ```

## 5. `dataset`
- **中文**：HTML5 自定义数据属性接口  
- **英文**：An interface to access custom data attributes (`data-*`).  
- **特性**：
  - 属性名自动转换（`data-user-id` → `userId`）
  - 值始终为字符串类型
  - 修改会实时同步到 DOM
- **示例**：
  ```html
  <div data-user-id="123" data-role="admin"></div>
  <script>
    const userId = element.dataset.userId; // "123"
    element.dataset.role = 'superuser'; // 修改属性
  </script>
  ```

## 注意事项
1. `querySelectorAll` 返回的是静态集合，如需动态查询应考虑其他方法
2. `classList` 方法在现代浏览器中已完全支持，IE10+ 支持基本功能
3. 事件监听器要避免内存泄漏，及时移除无用监听
4. `setTimeout` 的延迟时间不精确，不可依赖其做精确计时
5. `dataset` 操作会触发 DOM 重绘，频繁操作可能影响性能

<!-- by: Zou Jinyu (邹金玉) -->
```
