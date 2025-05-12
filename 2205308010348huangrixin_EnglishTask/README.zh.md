## 一、📮 我负责的部分1——卡片记忆游戏核心功能阐述与界面截图

#### 一、小组分工选择说明

```markdown
    <!-- by huangrixin -->
### 阐述：在小组任务中，我承担了第3.4部分的职责。
```

##### 1.截图--小组任务中第3.4部分

```markdown
![小组任务第3.4部分图像](D:\2205308010348huangrixin_EnglishFinalExperiment\images\huangrixinPart1.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\huangrixinPart1.png)

#### 二、任务--添加任务和已完成任务

##### 1.📝新增任务

```markdown
### 添加任务
### 项目主要功能说明任务
1. 设计和实现游戏界面：
   - **任务描述**：检查游戏布局。
   - **任务状态**：未完成 ❌
2. 实现卡片随机排列：
   - **任务描述**：每次游戏开始时，检查和判断卡片的位置是否会随机排列？
   - **任务状态**：未完成 ❌
3. 实现卡片翻牌逻辑：
   - **任务描述**：玩家可以多少翻张卡片查看图案，每次最多翻开多少张卡片？
   - **任务状态**：未完成 ❌
4. 实现卡片配对检查：
   - **任务描述**：卡片图案情况的翻开状态是如何的？
   - **任务状态**：未完成 ❌
5. 实现游戏结束条件：
   - **任务描述**：游戏结束条件是什么？
   - **任务状态**：未完成 ❌
6. 游戏重置功能：
   - **任务描述**：玩家重新开始游戏的方法是什么？
   - **任务状态**：未完成 ❌
7. 项目框架功能：
   - **任务描述**：项目框架主要功能是什么？主要包含哪些技术栈、主要组件或者重要模块？
   - **任务状态**：未完成 ❌
  -------------------------------------------------------------------------------------

```

##### 2.✅已完成任务勾选

```markdown
### 勾选已完成任务
### 项目主要功能说明任务
1. 设计和实现游戏界面：
   - **任务描述**：游戏界面由 4×3 的排列顺序，共有 12 张卡片，，每张卡片有两面（正面和反面）。
   - **任务状态**：已完成 ✅
2. 实现卡片随机排列：
   - **任务描述**：每次游戏开始时，卡片的位置会随机排列。
   - **任务状态**：已完成 ✅
3. 实现卡片翻牌逻辑：
   - **任务描述**：玩家可以翻开一张卡片查看图案，每次最多翻开两张卡片。
   - **任务状态**：已完成 ✅
4. 实现卡片配对检查：
   - **任务描述**：如果两张卡片图案相同，它们会保持翻开状态；如果不同，它们会恢复原样。
   - **任务状态**：已完成 ✅
5. 实现游戏结束条件：
   - **任务描述**：游戏结束条件是所有卡片成功配对。
   - **任务状态**：已完成 ✅
6. 添加游戏重置功能：
   - **任务描述**：直接刷新，玩家就可以重新开始游戏。
   - **任务状态**：已完成 ✅
7. 项目框架功能：
   - **任务描述**：项目框架主要功能说明。
   - **任务状态**：已完成 ✅
  -------------------------------------------------------------------------------------
   
```

#### 三、卡片记忆游戏项目主要功能说明

##### 1.项目主要功能说明及游戏玩法

```markdown
   - **这是一个简单的记忆卡片配对游戏，纯前端项目，无需后端依赖，可以直接在浏览器中运行。游戏玩法和项目游戏主要功能使用教程和说明：**
### 游戏玩法
  - 玩家可以任意翻开卡片，找到两两图案相同配对的卡片。每次翻开两张卡片，如果两张卡片匹配，则它们会保持翻开状态，同时，已经翻开的卡片无法再翻回背面；如果不匹配，则它们会翻回背面。玩家需要通过记忆卡片的位置和图案，当找到所有配对的卡片时，则游戏结束，即闯关成功。
### 游戏主要功能使用教程和说明
1. **游戏界面展示**：
   - 游戏界面由 4×3 的排列顺序，共有 12 张卡片，两两图案相同。
   - 每次游戏开始时，卡片的位置会随机排列。
2. **卡片配对逻辑**：
   - 玩家可以翻开任意一张卡片查看图案。
   - 每一轮最多翻开两张卡片，每一次最多只能翻开一张卡片。
   - 如果两张卡片图案相同，它们会保持翻开状态，同时，无法再翻回背面；如果不同，它们会恢复原样。
   - 游戏结束条件是所有卡片成功配对。
3. **游戏重置功能**：
   - 当刷新时，也就是每次重新开始游戏时，卡片的位置会随机排列。
```

##### 2.项目框架主要功能说明

```markdown
   cards-memory-game/              # 项目名称：卡片记忆游戏
├── .git/                          # Git 版本控制相关文件，用于管理代码版本
├── docs/                          # 项目文档
│   └── ...                        # 存放项目的设计文档、使用说明等
├── gameBase/                      # 游戏核心逻辑代码
│   └── ...                        # 包括游戏状态管理、卡片配对逻辑等
├── img/                           # 图像资源
│   └── ...                        # 存放游戏中使用的所有图像资源，包括卡片的正面和背面图案
├── NON_CODE_CONTRIBUTIONS/        # 非代码贡献相关内容
│   └── ...                        # 如设计、文档等
├── React/                         # React 相关代码（如果项目使用 React 构建）
│   └── ...                        # 存放 React 相关的组件和逻辑
├── Svelte/                        # Svelte 相关代码（如果项目使用 Svelte 构建）
│   └── ...                        # 存放 Svelte 相关的组件和逻辑
├── translation/                   # 多语言支持文件
│   └── ...                        # 存放多语言支持的文件，便于游戏支持多种语言
├── TypeScript/                    # TypeScript 代码（如果项目使用 TypeScript 编写）
│   └── ...                        # 存放 TypeScript 代码
├── VUE/                           # Vue 相关代码（如果项目使用 Vue 构建）
│   └── ...                        # 存放 Vue 相关的组件和逻辑
├── .gitignore                     # Git 忽略文件配置
│   └── ...                        # 指定哪些文件不被版本控制
├── CODE_OF_CONDUCT.md             # 项目行为准则
├── CONTRIBUTING.md                # 贡献指南
├── LICENSE                        # 开源许可证文件
├── README.md                      # 项目自述文件
│   └── ...                        # 包括项目介绍、安装和使用说明等
   > 1.**版本控制管理**
   >> 使用 Git 进行代码版本控制，确保代码的历史记录和协作开发。配置 Git 忽略某些不需要版本控制的文件。
   >> docs/: 存放项目的各类文档，包括设计文档、使用说明、架构图等，帮助开发者理解和使用项目。
  >> README.md: 项目的自述文件，提供项目介绍、安装和使用说明。
  >> CODE_OF_CONDUCT.md: 项目行为准则，规范贡献者的行为。
  >> CONTRIBUTING.md: 贡献指南，说明如何为项目做贡献。
  > 2.**游戏核心逻辑**
  >> gameBase/: 存放游戏的核心逻辑代码，包括游戏状态管理、卡片配对逻辑等。
  >> 游戏状态管理：管理游戏的不同状态，如初始化、进行中、结束等。
  >> 卡片配对逻辑：实现卡片配对的核心算法和规则。
  > 3.**图像资源管理**
  >> img/: 存放游戏中使用的所有图像资源，包括卡片的正面和背面图案。
  >> 非代码贡献、多语言支持
  >> NON_CODE_CONTRIBUTIONS: 存放非代码贡献相关的内容，如设计稿、文档、图像资源等。
  >> translation/: 存放多语言支持的文件，便于游戏支持多种语言，提升游戏的国际化水平。
  > 4.**前端框架支持**
  >> React、Svelte、VUE: 存放组件和逻辑。
  >> TypeScript 代码，提升代码的可维护性和类型安全性。
```

##### 3.截图--项目框架截图

```markdown
![项目框架](D:\2205308010348huangrixin_EnglishFinalExperiment\images\ProjectFramework.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\ProjectFramework.png)

##### 4.截图--项目游戏主要功能的界面截图：

```markdown
![项目界面截图-功能图1第一轮](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图1-第一轮.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图1-第一轮.png)

```markdown
![项目界面截图-功能图2第一轮](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图2-第一轮.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图2-第一轮.png)

```markdown
![项目界面截图-功能图3第二](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图3-第二轮.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图3-第二轮.png)

```markdown
![项目界面截图-功能图4第二](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图4-第二轮.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图4-第二轮.png)

```markdown
![项目界面截图-功能图5第二](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图5-第二轮.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图5-第二轮.png)

```markdown
![项目界面截图-功能图6第二](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图6-第二轮.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图6-第二轮.png)

```markdown
![项目界面截图-功能图7第三](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图7-第三轮.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图7-第三轮.png)

```markdown
![项目界面截图-功能图8第四](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图8-第四轮.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图8-第四轮.png)

```markdown
![项目界面截图-功能图9第五](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图9-第五轮.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图9-第五轮.png)

```markdown
![项目界面截图-功能图10游戏结束第六](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图10-第六轮(闯关成功游戏结束).png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图10-第六轮(闯关成功游戏结束).png)

```markdown
![项目界面截图-功能图11刷新浏览器页面，随机排序，游戏重新开始](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图11-刷新浏览器页面，随机排列.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图11-刷新浏览器页面，随机排列.png)

<!-- by huangrixin -->



## 二、📦 我负责的部分2——卡片记忆游戏项目框架中TypeScript文件说明

#### 一、小组分工选择说明

```markdown
    <!-- by huangrixin -->
### 阐述：在小组任务中，我承担了第五部分，项目里面的文件具体包含：MemoryCard.tsx、App.css、main.tsx、tsconfig.json的职责。
```

##### 1.截图--我承担了小组任务中第五部分

```markdown
![小组任务第五部分图像](D:\2205308010348huangrixin_EnglishFinalExperiment\images\huangrixinPart2.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\huangrixinPart2.png)

#### 二、任务--📝添加任务和✅已完成任务

##### 1.添加任务和已完成任务

```markdown
  1. ✅ 能解释游戏核心玩法机制
  2. ✅ 能描述卡片翻转的CSS实现原理
  3. ✅ 能说明组件间的数据流动
  4. ✅ 能指出状态管理的设计方式
  5. ✅ 能识别项目的可扩展点
  6. ✅ 能说明性能优化点
  -  ✅**总结**：项目框架中TypeScript任务，MemoryCard.tsx、App.css、main.tsx、tsconfig.json文件源代码了解和说明。

```

#### 三、源代码文件主要了解和说明

##### 1. 核心功能理解及关键代码分析

```markdown
## 1. MemoryCard.tsx 
  - **主要功能**：卡片组件，负责渲染每张记忆卡片并处理卡片的翻转逻辑。
  - **代码说明**：MemoryCard 组件接收 MemoryCardProps 类型的属性，包括 isEnable、handleClick、index、image、name、isDone 和 isOpen。flipCard 函数用于处理卡片的点击事件，只有在卡片可用时（isEnable 为 true）才会触发。根据 isDone 和 isOpen 状态，组件决定是否翻转卡片。卡片由两个 img 元素组成，分别表示卡片的正面和背面。
  - **关键代码**：
export const MemoryCard = (props: MemoryCardProps) => {
  const flipCard = () => {
    if (props.isEnable) {
      props.handleClick(props.index);
    }
  }
  return props.isDone ? (
    <div className="memory-card flip">...</div> 
  ) : (
    <div className={`memory-card ${props.isOpen && 'flip'}`} onClick={flipCard}>...</div>
  )
}
  -------------------------------------------------------------------------------------
## 2. App.css 
  - **主要功能**：全局样式文件，定义了应用的整体样式布局。
  - **代码说明**：.memory-game 定义了游戏容器的布局，使用 Flexbox 布局来排列卡片。.memory-card 定义了卡片的基本样式，包括大小、位置和动画效果。.memory-card.flip 定义了卡片翻转时的样式，通过 transform: rotateY(180deg) 实现翻转效果。
  - **关键代码**：
.memory-game {
  width: 640px;
  height: 640px;
  margin: auto;
  display: flex;
  flex-wrap: wrap;
  perspective: 1000px;
}

.memory-card {
  width: calc(25% - 10px);
  height: calc(33.333% - 10px);
  margin: 5px;
  position: relative;
  transform-style: preserve-3d;
  transition: transform 0.5s;
}

.memory-card.flip {
  transform: rotateY(180deg);
}
  -------------------------------------------------------------------------------------
## 3. main.tsx 
  - **主要功能**：负责将 React 应用程序渲染到 DOM 中。
  - **代码说明**：使用 ReactDOM.createRoot 将 React 应用程序渲染到 document.getElementById('root') 元素中。<React.StrictMode> 用于启用 React 的严格模式，帮助识别潜在的问题。<App /> 是应用程序的根组件。
  - **关键代码**：
ReactDOM.createRoot(document.getElementById('root') as HTMLElement).render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);
  -------------------------------------------------------------------------------------
## 4. tsconfig.json 
  - **主要功能**：配置 TypeScript 编译器的选项。
  - **代码说明**："target": "ESNext" 指定 TypeScript 编译为最新的 JavaScript 特性。"strict": true 启用严格模式，帮助捕获常见的编程错误。"jsx": "react-jsx" 指定使用 React 的 JSX 转换。"include": ["src"] 指定包含在编译中的源文件目录。
  - **关键代码**：
{
  "compilerOptions": {
    "jsx": "react-jsx"
    "strict": true
    "moduleResolution": "Node"
  }
}
```

##### 2. 关键算法与数据结构

```markdown
  - **算法**：卡片匹配算法。
  - **代码**：
function handleCardClick(index) {
  if (selectedCards.length < 2) {
    const newState = [...selectedCards, index];
    if (newState.length === 2 && cards[newState[0]] === cards[newState[1]]) {
      setMatchedCards([...matchedCardsnewState]);
    }
    
    setSelectedCards(newState);
  }
}
```

##### 3. 状态管理流程

```markdown
### 状态管理流程
1. 卡片初始状态：背面朝上(显示JavaScript图标)
2. 用户点击 → 触发'flipCard' → 调用父组件'handleClick'。
3. 根据'isOpen'状态决定是否显示正面图案.
4. 匹配成功后'isDone'为true，保持正面显示.
```

##### 4. 项目扩展性

```markdown
###  项目扩展性
  - 多框架支持：项目结构已预留React/Svelte/Vue等不同实现.
  - 国际化支持：存在translation目录用于多语言
  - 资源管理：img目录集中管理所有卡片图案
```

##### 5. 项目意义

```markdown
###  项目意义
1. TypeScript强类型：明确定义组.
2. 教育价值：适合用于前端教学和前端新手.
3. 设计模式实践：展示组件通信和状态管理.
4. 跨平台潜力：项目结构支持扩展到Web/Mobile.
```

##### 6. 性能优化点

```markdown
### 性能优化点
  - 硬件加速：通过 transform属性触发GPU加速.
  - 内存优化：使用函数组件减少实例开销.
  - 动画性能：CSS transition优于JavaScript动画.
```

<!-- by huangrixin -->

