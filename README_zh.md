## I. 📮项目主要功能描述与截图

#### 1. 小组任务分工选择说明

```markdown
### 说明：我选择了小组任务的第 3.4 部分。
```

##### 1.截图--小组任务中第3.4部分原图

```markdown
![小组任务中的第 3.4 部分](D:\University - Huang Rixin\English Major Practice\Instructions/Division_of_Work_1.png)
```

![](D:\University - Huang Rixin\English Major Practice\Files_to_Submit/Division_of_Work_1-1746875616391.png)

#### 2.任务

##### 1. 添加任务

```markdown
### 添加任务  
### 项目主要功能描述任务  
1. 设计并实现游戏界面：  
   - **任务描述**：评审并完善游戏布局方案。  
   - **任务状态**：未完成 ❌  
2. 实现卡片随机排列：  
   - **任务描述**：确保每次游戏启动时卡片位置随机初始化。  
   - **任务状态**：未完成 ❌  
3. 实现卡片翻转逻辑：  
   - **任务描述**：明确玩家单次可翻转卡片数量及最大并发翻转限制。  
   - **任务状态**：未完成 ❌  
4. 实现卡片配对检查：  
   - **任务描述**：定义卡片翻转后不同匹配状态的视觉表现与交互逻辑。  
   - **任务状态**：未完成 ❌  
5. 实现游戏结束条件：  
   - **任务描述**：制定游戏胜利/失败的完整判定规则。  
   - **任务状态**：未完成 ❌  
6. 游戏重置功能：  
   - **任务描述**：设计并实现游戏状态完全重置的触发机制。  
   - **任务状态**：未完成 ❌  
7. 项目框架功能：  
   - **任务描述**：梳理项目架构的核心功能模块、技术选型及依赖关系。  
   - **任务状态**：未完成 ❌  

--------------------------------------------------  

### 项目框架中的 TypeScript 任务  
- **任务描述**：深入解析 MemoryCard.tsx、App.css、main.tsx 和 tsconfig.json 文件的实现原理与设计模式。  
- **任务状态**：未完成 ❌  
```

##### 2. 标记已完成任务

```markdown
### 标记已完成任务
#### 项目主要功能描述任务
1. **设计并实现游戏界面**  
   - **任务描述**：游戏界面采用4×3网格布局，共12张卡片，每张卡片均有正反两面。  
   - **任务状态**：已完成 ✅  

2. **实现卡片随机排列**  
   - **任务描述**：每次游戏启动时，卡片位置会随机排列。  
   - **任务状态**：已完成 ✅  

3. **实现卡片翻转逻辑**  
   - **任务描述**：玩家每次可翻转一张卡片查看图案，每轮最多可翻转两张卡片。  
   - **任务状态**：已完成 ✅  

4. **实现卡片配对检查**  
   - **任务描述**：若两张卡片图案一致，则保持翻转状态；若不一致，则恢复初始状态。  
   - **任务状态**：已完成 ✅  

5. **实现游戏结束条件**  
   - **任务描述**：当所有卡片成功配对时，游戏结束。  
   - **任务状态**：已完成 ✅  

6. **添加游戏重置功能**  
   - **任务描述**：玩家刷新页面即可重新开始游戏。  
   - **任务状态**：已完成 ✅  

7. **项目框架功能**  
   - **任务描述**：项目框架的主要功能如下：  
     1. **版本控制管理**  
        - 使用Git进行代码版本控制，确保代码可追溯性和协作开发。配置Git忽略无需版本控制的文件。  
        - `docs/`：存放项目文档（设计文档、使用说明、架构图等）。  
        - `README.md`：项目自述文件，包含介绍、安装和使用说明。  
        - `CODE_OF_CONDUCT.md`：项目行为准则，规范贡献者行为。  
        - `CONTRIBUTING.md`：贡献指南，说明如何参与项目。  

     2. **游戏核心逻辑**  
        - `gameBase/`：存放游戏核心逻辑（状态管理、配对算法等）。  
        - 游戏状态管理：处理初始化、进行中、结束等状态。  
        - 卡片配对逻辑：实现匹配判定规则。  

     3. **图像资源管理**  
        - `img/`：存放所有卡片正反面图案资源。  
        - 国际化支持：  
          - `NON_CODE_CONTRIBUTIONS/`：存放设计草图、文档等非代码资源。  
          - `translation/`：存放多语言支持文件，提升国际化水平。  

     4. **前端框架支持**  
        - 支持React、Svelte、Vue等框架组件。  
        - 使用TypeScript编写，增强代码可维护性和类型安全。  
   - **任务状态**：已完成 ✅  

--------------------------------------

#### 项目框架中的TypeScript任务  
- **任务描述**：深入解析MemoryCard.tsx、App.css、main.tsx和tsconfig.json文件的实现原理与设计模式，具体详见 -- II. 项目框架中的TypeScript文件夹任务。  
- **任务状态**：已完成 ✅  
```

#### 3. 项目主要功能描述

##### 1. 项目主要功能描述与游戏玩法

```markdown
- **这是一款简单的记忆卡片配对游戏，纯前端项目，无需后端依赖，可直接在浏览器中运行。游戏玩法及项目主要功能使用教程与说明**：

### 游戏玩法
- 玩家可自由翻转卡片以寻找图案相同的配对。每次翻转两张卡片，若匹配则保持翻开状态且不可再翻转；若不匹配则恢复原状。玩家需记住卡片位置与图案。当所有卡片成功配对时，游戏结束，即成功通关。

### 游戏主要功能使用教程与说明
1. **游戏界面显示**
   - 游戏界面为4×3网格布局，共12张卡片，配对卡片图案相同。
   - 每次游戏启动时，卡片位置随机排列。

2. **卡片配对逻辑**
   - 玩家可任意翻转卡片查看图案。
   - 每轮最多翻转两张卡片，每次仅能翻转一张。
   - 若两张卡片图案相同，则保持翻开状态且不可再翻转；若不同则恢复原状。
   - 当所有卡片成功配对时，游戏结束。

3. **游戏重置功能**
   - 刷新页面重新开始游戏时，卡片位置将再次随机排列。
```

##### 2. 项目框架主要功能描述

```markdown
cards-memory-game/              # 项目名称：卡片记忆游戏
├── .git/                          # Git 版本控制相关文件，用于管理代码版本
├── docs/                          # 项目文档
│   └── ...                        # 存储项目设计文档、使用说明等
├── gameBase/                      # 游戏核心逻辑代码
│   └── ...                        # 包括游戏状态管理、卡片配对逻辑等
├── img/                           # 图像资源
│   └── ...                        # 存储游戏中使用的所有图像资源，包括卡片的正面和背面图案
├── NON_CODE_CONTRIBUTIONS/        # 非代码贡献相关内容
│   └── ...                        # 如设计、文档等
├── React/                         # React 相关代码（如果项目使用 React 构建）
│   └── ...                        # 存储 React 相关组件和逻辑
├── Svelte/                        # Svelte 相关代码（如果项目使用 Svelte 构建）
│   └── ...                        # 存储 Svelte 相关组件和逻辑
├── translation/                   # 多语言支持文件
│   └── ...                        # 存储多语言支持文件，便于游戏支持多种语言
├── TypeScript/                    # TypeScript 代码（如果项目使用 TypeScript 编写）
│   └── ...                        # 存储 TypeScript 代码
├── VUE/                           # Vue 相关代码（如果项目使用 Vue 构建）
│   └── ...                        # 存储 Vue 相关组件和逻辑
├── .gitignore                     # Git 忽略文件配置
│   └── ...                        # 指定哪些文件不进行版本控制
├── CODE_OF_CONDUCT.md             # 项目行为准则
├── CONTRIBUTING.md                # 贡献指南
├── LICENSE                        # 开源许可证文件
├── README.md                      # 项目自述文件
│   └── ...                        # 包括项目介绍、安装和使用说明等
   1. 版本控制管理：
   - 使用 Git 进行代码版本控制，以确保代码的历史记录和协作开发。配置 Git 忽略某些不需要版本控制的文件。
   - docs/：存储各种项目文档，包括设计文档、使用说明、架构图等，以帮助开发人员理解和使用项目。
   - README.md：项目的自述文件，提供项目介绍、安装和使用说明。
   - CODE_OF_CONDUCT.md：项目的行为准则，规范贡献者的行为。
   - CONTRIBUTING.md：贡献指南，解释如何为项目做出贡献。
   2. 游戏核心逻辑
   - gameBase/：存储游戏的核心逻辑代码，包括游戏状态管理、卡片配对逻辑等。
   - 游戏状态管理：管理游戏的不同状态，如初始化、进行中、结束。
   - 卡片配对逻辑：实现卡片配对的核心算法和规则。
   3. 图像资源管理
   - img/：存储游戏中使用的所有图像资源，包括卡片的正面和背面图案。
   - 非代码贡献、多语言支持
   - NON_CODE_CONTRIBUTIONS：存储与非代码贡献相关的内容，如设计草图、文档、图像资源等。
   - translation/：存储多语言支持文件，便于游戏支持多种语言，提高其国际化水平。
   4. 前端框架支持
   - React、Svelte、VUE：存储组件和逻辑。
   - TypeScript 代码，增强代码的可维护性和类型安全性。
```

##### 3. 项目框架截图

```markdown
![项目框架](D: \ 2205308010348 Huang Rixin \ English Professional Practice \ images \ Project Framework. png)
```

##### ![](D:\2205308010348黄日欣\英语专业实践\images\项目框架.png)

##### 4.项目游戏界面主要功能截图：

```markdown
![功能图 1 - 第一轮](D:\2205308010348 Huang Rixin\English Major Practical Training/Feature_Image_1-Round_1.png)
```

##### ![](D:\2205308010348黄日欣\英语专业实践/功能图1-第一轮-1746879573153.png)

```markdown
![功能图 2 - 第一轮](D:\2205308010348 Huang Rixin\English Major Practical Training/Feature_Image_2-Round_1.png)
```

##### ![](D:\2205308010348黄日欣\英语专业实践/功能图2-第一轮-1746879585707.png)

```markdown
![功能图 3 - 第二轮](D:\2205308010348 Huang Rixin\English Major Practical Training/Feature_Image_3-Round_2.png)
```

##### ![](D:\2205308010348黄日欣\英语专业实践/功能图3-第二轮-1746879598373.png)

```markdown
![功能图 4 - 第二轮](D:\2205308010348 Huang Rixin\English Major Practical Training/Feature_Image_4-Round_2.png)
```

##### ![](D:\2205308010348黄日欣\英语专业实践/功能图4-第二轮-1746879606935.png)

```markdown
![功能图 5 - 第二轮](D:\2205308010348 Huang Rixin\English Major Practical Training/Feature_Image_5-Round_2.png)
```

##### ![](D:\2205308010348黄日欣\英语专业实践/功能图5-第二轮-1746879615845.png)

```markdown
![功能图 6 - 第二轮](D:\2205308010348 Huang Rixin\English Major Practical Training/Feature_Image_6-Round_2.png)
```

![](D:\2205308010348黄日欣\英语专业实践/功能图6-第二轮-1746879626024.png)

```markdown
![功能图 7 - 第三轮](D:\2205308010348 Huang Rixin\English Major Practical Training/Feature_Image_7-Round_3.png)
```

![](D:\2205308010348黄日欣\英语专业实践/功能图7-第三轮-1746879638441.png)

```markdown
![功能图 8 - 第四轮](D:\2205308010348 Huang Rixin\English Major Practical Training/Feature_Image_8-Round_4.png)
```

![](D:\2205308010348黄日欣\英语专业实践/功能图8-第四轮-1746879646549.png)

```markdown
![功能图 9 - 第五轮](D:\2205308010348 Huang Rixin\English Major Practical Training/Feature_Image_9-Round_5.png)
```

![](D:\2205308010348黄日欣\英语专业实践/功能图9-第五轮-1746879657288.png)

```markdown
![功能图 10 - 第六轮（闯关成功，游戏结束）](D:\2205308010348 Huang Rixin\English Major Practical Training/Feature_Image_10-Round_6_(Level_Cleared,_Game_Over).png)
```

![](D:\2205308010348黄日欣\英语专业实践/功能图10-第六轮(闯关成功游戏结束)-1746879663711.png)

```markdown
![功能图 11 - 刷新浏览器页面以随机排列并重新开始游戏](D:\2205308010348 Huang Rixin\English Major Practical Training/Feature_Image_11-Refresh_Browser_Page_to_Shuffle_Randomly.png)
```

![](D:\2205308010348黄日欣\英语专业实践/功能图11-刷新浏览器页面，随机排列-1746879675157.png)

<!-- by liyueying -->

## II. 项目框架中的 TypeScript 文件描述

#### 1. 小组任务分工选择说明

```markdown
### 说明：我选择了小组任务的第 5 部分。这部分项目包含的文件有：MemoryCard.tsx、App.css、main.tsx 和 tsconfig.json。
```

##### 1. 小组任务中所选第 5 部分的原始截图

```markdown
![小组任务的第 3.4 部分](D: \ 2205308010348 Huang Rixin \ English Professional Practice \ images \ My Responsibility Part 2. png)
```

![](D:\2205308010348黄日欣\英语专业实践\images\我负责的部分2.png)

#### 2. 任务

##### 1.已添加任务和已完成任务

```markdown
  1. ✅ 能够解释游戏的核心玩法机制
  2. ✅ 能够描述卡片翻转的 CSS 实现原理
  3. ✅ 能够解释组件之间的数据流
  4. ✅ 能够识别状态管理的设计方法
  5. ✅ 能够识别项目的可扩展性点
  6. ✅ 能够解释性能优化点
```

#### 3. 源代码文件主要说明

##### 1. 核心功能理解和关键代码分析

```
## 1. MemoryCard.tsx 
  - **主要功能**：卡片组件，负责渲染每张记忆卡片并处理卡片翻转逻辑。
  - **代码解释**：MemoryCard 组件接收 MemoryCardProps 类型的属性，包括 isEnable、handleClick、index、image、name、isDone 和 isOpen。flipCard 函数处理卡片点击事件，仅当卡片启用（isEnable 为 true）时触发。根据 isDone 和 isOpen 状态，组件决定是否翻转卡片。卡片由两个 img 元素组成，分别代表卡片的正面和背面。
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
  ---------------------------------------
## 2. App.css 
  - **主要功能**：全局样式文件，定义应用程序的整体布局和样式。
  - **代码解释**：.memory-game 使用 Flexbox 定义游戏容器的布局，用于排列卡片。.memory-card 定义卡片的基本样式，包括大小、位置和动画效果。.memory-card.flip 定义卡片翻转时的样式，通过 transform: rotateY(180deg) 实现翻转效果。
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
  --------------------------------
## 3. main.tsx 
  - **主要功能**：负责将 React 应用程序渲染到 DOM 中。
  - **代码解释**：使用 ReactDOM.createRoot 将 React 应用程序渲染到通过 document.getElementById('root') 获取的元素中。<React.StrictMode> 用于启用 React 的严格模式，有助于识别潜在问题。<App /> 是应用程序的根组件。
  - **关键代码**：
ReactDOM.createRoot(document.getElementById('root') as HTMLElement).render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);
  ----------------------------
## 4. tsconfig.json 
  - **主要功能**：配置 TypeScript 编译器的选项。
  - **代码解释**："target": "ESNext" 指定 TypeScript 应编译为最新的 JavaScript 特性。"strict": true 启用严格模式，有助于捕获常见的编程错误。"jsx": "react-jsx" 指定使用 React 的 JSX 转换。"include": ["src"] 指定要包含在编译中的源文件目录。
  - **关键代码**：
{
  "compilerOptions": {
    "jsx": "react-jsx",
    "strict": true,
    "moduleResolution": "Node"
  }
}
```

##### 2. 关键算法和数据结构

```markdown
- **算法**：卡片匹配算法。
  - **代码**：
function handleCardClick(index) {
  if (selectedCards.length < 2) {
    const newState = [...selectedCards, index];
    if (newState.length === 2 && cards[newState[0]] === cards[newState[1]]) {
      setMatchedCards([...matchedCards, newState]);
    }
    
    setSelectedCards(newState);
  }
}
```

##### 3. 状态管理流程

```markdown
### 状态管理流程
  1. 初始卡片状态：面朝下（显示 JavaScript 图标）
  2. 用户点击 → 触发 'flipCard' → 调用父组件的 'handleClick'。
  3. 根据 'isOpen' 状态确定是否显示正面图片。
  4. 成功匹配后，'isDone' 变为 true，保持正面图片显示。
```

##### 4. 项目可扩展性

```markdown
### 项目可扩展性
- 多框架支持：项目结构已为 React/Svelte/Vue 等不同实现做好准备。
- 国际化支持：存在 translation 目录以支持多语言。
- 资源管理：img 目录集中管理所有卡片图像。
```

##### 5.  项目意义

```markdown
### 项目意义
1. TypeScript 强类型：明确定义组件类型。
2. 教育价值：适用于前端教学和前端开发初学者。
3. 设计模式实践：展示组件通信和状态管理。
4. 跨平台潜力：项目结构支持扩展到 Web/移动平台。
```

##### 6. 性能优化点

```markdown
### 性能优化点
  - 硬件加速：通过 transform 属性触发 GPU 加速。
  - 内存优化：使用函数式组件减少实例开销。
  - 动画性能：CSS 过渡优于 JavaScript 动画。
```

<!-- by liyueying-->
