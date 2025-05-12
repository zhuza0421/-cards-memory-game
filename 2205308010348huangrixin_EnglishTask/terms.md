## 1. Card Memory Game：Project terminology (keywords) in English

```markdown
### 1.MemoryCard
  -  Chinese: Memory Card Component
  - English: Memory Card Component
  - Explanation: A component defined in React, used to represent each memory card in the game. This component receives properties (such as image, whether it has been flipped, whether it has been matched, etc.) passed from its parent component and renders the card's appearance and behavior based on these properties.
### 2.addEventListener
  - Chinese: Add Event Listener
  - English: Registers the specified listener on the EventTarget it's called on.
  - Explanation: Used to add an event listener to an element, allowing a corresponding function to be executed when a specific event occurs. In the memory card game, this function is used to add a click event listener to the card, triggering the flip logic when the player clicks on it.
### 3.style.order
  - Chinese: Set the Order of a Flex Item
  - English: Sets the order of a flex item in its flex container.
  - Explanation: Used to set the order of elements within a flex container. In the memory card game, the style.order property of each card can be set to randomly arrange the cards' positions, increasing the game's challenge and fun.
### 4.flipCard
  - Chinese: Flip Card Function
  - English: A function to flip a memory card.
  - Explanation: Used to handle the flip logic when a card is clicked. This function determines whether the card is the first one flipped and whether it matches the previously flipped card. Based on the judgment, the function decides whether to keep the card flipped or flip it back to its back.
### 5.transform-style
  - Chinese: Transform Style Property
  - English: The transform-style CSS property sets whether children of an element are positioned in the 3D-space or are flattened in the plane of the element.
  - Explanation: Used in CSS to control whether child elements are transformed in 3D space. In the memory card game, setting transform-style: preserve-3d maintains the 3D transformation effect of the memory cards, providing a more realistic 3D visual effect when flipping the cards.
### 6.perspective
  - Chinese: Perspective Property
  - English: Perspective Property
  - Explanation: A CSS property used to set the perspective effect of 3D elements, i.e., the distance between the observer and the z=0 plane. In the memory card game, setting the perspective property of the game container enhances the 3D visual effect, giving the cards a more pronounced sense of depth when flipped.
### 7.backface-visibility
  - Chinese: Backface Visibility Property
  - English: Backface Visibility Property
  - Explanation: A CSS property used to control whether the back face of an element is visible when rotated. In the memory card game, setting the card's back face to backface-visibility: hidden ensures that the back face is not visible when rotated, achieving the flip effect.
### 8.flex-wrap
  - Chinese: Flex Wrap Property
  - English: The flex-wrap CSS property sets whether flex items are forced onto one line or can wrap onto multiple lines.
  - Explanation: Used in CSS to control whether elements within a flex container wrap. In the memory card game, setting the game container's flex-wrap property to wrap allows the memory cards to automatically wrap within the container, adapting to different screen sizes and card quantities.
### 9.className
  - Chinese: CSS Class Name Attribute
  - English: The CSS class name attribute
  - Explanation: Used in React to set the CSS class name of an element. In the memory card game, the className property of the card is dynamically set based on its state (such as whether it has been flipped, whether it has been matched, etc.), thereby changing the card's appearance and behavior.
### 10.props
  - Chinese: 组件属性 (Component Properties)
  - English: Properties passed to a component
  - Explanation: In React, props are used to pass data from a parent component to a child component. In the memory card game, the parent component (such as the main game component) passes the properties of the memory cards (such as image, whether it has been flipped, whether it has been matched, etc.) to the MemoryCard component via props, enabling the MemoryCard component to correctly render and display the cards.
    -------------------------------------------------------------------------------------
```

<!-- by huangrixin -->

## 2.卡片记忆游戏：项目术语（关键字）中文

```markdown
### 1. MemoryCard
  - 中文: 记忆卡片组件
  - 英文: Memory Card Component
  - 解释: 在React中定义的组件，用于表示游戏中的每一张记忆卡片。该组件接收父组件传递的属性（如图片、是否已翻开、是否已完成配对等），并根据这些属性来渲染卡片的外观和行为。
### 2. addEventListener
  - 中文: 添加事件监听器
  - 英文: Registers the specified listener on the EventTarget it's called on.
  - 解释: 用于为元素添加事件监听器，以便在特定事件发生时执行相应的函数。在记忆卡片游戏中，这个函数用于为卡片添加点击事件监听器，以便在玩家点击卡片时触发翻牌逻辑。
### 3. style.order
  - 中文: 设置元素的排列顺序
  - 英文: Sets the order of a flex item in its flex container.
  - 解释: 用于设置flex容器中元素的排列顺序。在记忆卡片游戏中，可以通过设置每张卡片的style.order属性来随机排列卡片的位置，增加游戏的挑战性和趣味性。
### 4. flipCard
  - 中文: 翻牌函数
  - 英文: A function to flip a memory card.
  - 解释: 用于处理卡片被点击时的翻牌逻辑。该函数会判断卡片是否为第一张翻开的卡片，以及是否与之前翻开的卡片匹配。根据判断结果，函数会决定是否保持卡片翻开状态或将其翻回背面。
### 5. transform-style
  - 中文: 变换样式属性
  - 英文: The transform-style CSS property sets whether children of an element are positioned in the 3D-space or are flattened in the plane of the element.
  - 解释: 在CSS中用于控制子元素是否在3D空间中进行变换。在记忆卡片游戏中，设置transform-style: preserve-3d可以保持记忆卡片的3D变换效果，使卡片在翻牌时具有更真实的3D视觉效果。
### 6. perspective
  - 中文: 透视属性
  - 英文: Perspective Property
  - 解释: CSS属性，用于设置3D元素的透视效果，即观察者与z=0平面的距离。在记忆卡片游戏中，通过设置游戏容器的perspective属性，可以增强3D视觉效果，使卡片在翻牌时具有更明显的立体感。
### 7. backface-visibility
  - 中文: 背面可见性
  - 英文: Backface Visibility Property
  - 解释: CSS属性，用于控制元素背面在旋转时是否可见。在记忆卡片游戏中，将卡片的背面设置为backface-visibility: hidden，可以确保卡片背面在旋转时不可见，从而实现翻牌效果。
### 8. flex-wrap
  - 中文: Flex容器换行属性
  - 英文: The flex-wrap CSS property sets whether flex items are forced onto one line or can wrap onto multiple lines.
  - 解释: 在CSS中用于控制flex容器内的元素是否换行。在记忆卡片游戏中，通过设置游戏容器的flex-wrap属性为wrap，可以使记忆卡片在容器内自动换行排列，从而适应不同屏幕尺寸和卡片数量。
### 9. className
  - 中文: CSS类名属性
  - 英文: The CSS class name attribute
  - 解释: 在React中用于设置元素的CSS类名。在记忆卡片游戏中，根据卡片的状态（如是否已翻开、是否已完成配对等）动态设置卡片的className属性，从而改变卡片的外观和行为。
### 10. props
  - 中文: 组件属性
  - 英文: Properties passed to a component
  - 解释: 在React中，props用于从父组件向子组件传递数据。在记忆卡片游戏中，父组件（如游戏主组件）通过props向MemoryCard组件传递记忆卡片的属性（如图片、是否已翻开、是否已完成配对等），以便MemoryCard组件能够正确渲染和显示卡片。
  
    <!-- by huangrixin -->
```

