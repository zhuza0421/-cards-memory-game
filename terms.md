```markdown
# Web 前端开发核心术语

以下是五个关键技术的详细说明：

## 1. `querySelectorAll`
- **中文**：DOM 元素选择方法  
- **英文**：A DOM method that selects all elements matching a specified CSS selector and returns a NodeList.  
- **解释**：  
  用于通过 CSS 选择器获取文档中所有匹配的元素，返回一个静态的 `NodeList` 集合。  
  ```javascript
  // 示例用法
  document.querySelectorAll('.btn');
  ```

## 2. `classList`
- **中文**：HTML 元素的类名操作接口  
- **英文**：An interface for manipulating the class attributes of an HTML element.  
- **解释**：  
  提供以下常用方法动态修改元素类名：  
  - `add()` 添加类  
  - `remove()` 移除类  
  - `toggle()` 切换类  
  ```javascript
  // 示例：切换高亮状态
  element.classList.toggle('active');
  ```

## 3. `addEventListener`
- **中文**：事件监听方法  
- **英文**：A method to attach an event handler to an element.  
- **解释**：  
  支持的事件类型包括：  
  - `click` 点击事件  
  - `keydown` 按键事件  
  - `mouseover` 鼠标悬停  
  ```javascript
  // 示例：点击事件监听
  button.addEventListener('click', handleClick);
  ```

## 4. `setTimeout`
- **中文**：定时器函数  
- **英文**：A function that executes a callback after a specified delay (in milliseconds).  
- **特点**：  
  - 异步执行  
  - 可通过 `clearTimeout()` 取消  
  ```javascript
  // 示例：延迟1秒执行
  setTimeout(() => console.log('Done'), 1000);
  ```

## 5. `dataset`
- **中文**：HTML5 自定义数据属性访问方式  
- **英文**：An interface to access custom data attributes (`data-*`) of an element.  
- **用法说明**：  
  ```html
  <!-- HTML定义 -->
  <div data-user-id="123" data-role="admin"></div>
  
  <!-- JavaScript访问 -->
  <script>
    const role = element.dataset.role; // "admin"
  </script>
  ```
 
<!--by zoujinyu-->
<!--by 邹金玉-->

