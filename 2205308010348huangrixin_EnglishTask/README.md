## I.📮 Card Memory Game:Part 1 that I am responsible for - Main Function Description and Screenshots of the Project

#### 一、 Explanation of Group Task Division Selection

```markdown
    <!-- by huangrixin -->
### Explanation: I am responsible for section 3.4 of the group task.
```

##### 1. Screenshot - Original Image of Section 3.4 in the Group Task

```markdown
![GroupTaskSection3and4](D:\2205308010348huangrixin_EnglishFinalExperiment\images\huangrixinPart1.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\huangrixinPart1.png)

#### 二、Tasks-Add tasks and completed tasks

##### 1. Adding Tasks

```markdown
### Adding Tasks
### Project Main Function Description Tasks
1. Design and Implement the Game Interface:
   - **Task Description**: Review the game layout.
   - **Task Status**: Incomplete ❌
2. Implement Random Card Arrangement:
   - **Task Description**: Upon starting each game, check and determine if the card positions are randomly arranged?
   - **Task Status**: Incomplete ❌
3. Implement Card Flipping Logic:
   - **Task Description**: How many cards can the player flip to view the images? What is the maximum number of cards that can be flipped at a time?
   - **Task Status**: Incomplete ❌
4. Implement Card Pairing Check:
   - **Task Description**: What is the state of the cards when their images are revealed?
   - **Task Status**: Incomplete ❌
5. Implement Game End Conditions:
   - **Task Description**: What are the conditions for ending the game?
   - **Task Status**: Incomplete ❌
6. Game Reset Functionality:
   - **Task Description**: How can the player restart the game?
   - **Task Status**: Incomplete ❌
7. Project Framework Functionality:
   - **Task Description**: What are the main functions of the project framework? What technology stacks, main components, or important modules does it include?
   - **Task Status**: Incomplete ❌
  -------------------------------------------------------------------------------------

```

##### 2. Checking Off Completed Tasks

```markdown
### Checking Off Completed Tasks
#### Project Main Function Description Tasks
1. Design and Implement the Game Interface:
   - **Task Description**: The game interface consists of a 4×3 grid, totaling 12 cards. Each card has two sides (front and back).
   - **Task Status**: Completed ✅
2. Implement Random Card Arrangement:
   - **Task Description**: Upon starting each game, the card positions are randomly arranged.
   - **Task Status**: Completed ✅
3. Implement Card Flipping Logic:
   - **Task Description**: The player can flip one card to view the image, with a maximum of two cards flipped at a time.
   - **Task Status**: Completed ✅
4. Implement Card Pairing Check:
   - **Task Description**: If two cards have the same image, they remain flipped; if not, they return to their original state.
   - **Task Status**: Completed ✅
5. Implement Game End Conditions:
   - **Task Description**: The game ends when all cards are successfully paired.
   - **Task Status**: Completed ✅
6. Add Game Reset Functionality:
   - **Task Description**: The player can restart the game by simply refreshing the page.
   - **Task Status**: Completed ✅
7. Project Framework Functionality:
   - **Task Description**: The main functions of the project framework are described below:
   > 1.Version Control Management:
   >> Use Git for code version control to ensure the history and collaborative development of the code. Configure Git to ignore certain files that do not require version control.
   >> docs/: Stores various project documents, including design documents, usage instructions, architecture diagrams, etc., to help developers understand and use the project.
   - README.md: The project's self-explanatory file, providing an introduction to the project, installation, and usage instructions.
   - CODE_OF_CONDUCT.md: The project's code of conduct, regulating the behavior of contributors.
   >> CONTRIBUTING.md: Contribution guidelines, explaining how to contribute to the project.
   > 2.Game Core Logic
   >> gameBase/: Stores the core logic code of the game, including game state management, card pairing logic, etc.
   >> Game State Management: Manages different states of the game, such as initialization, in-progress, and end.
   >> Card Pairing Logic: Implements the core algorithms and rules for card pairing.
   > 3.Image Resource Management
   >> img/: Stores all image resources used in the game, including the front and back patterns of the cards.
   >> Non-Code Contributions, Multilingual Support
   >> NON_CODE_CONTRIBUTIONS: Stores content related to non-code contributions, such as design drafts, documents, image resources, etc.
   >> translation/: Stores files for multilingual support, facilitating the game's support for multiple languages and enhancing its internationalization level.
   > 4.Frontend Framework Support
   >> React, Svelte, VUE: Stores components and logic.
   >> TypeScript code, enhancing code maintainability and type safety.
   - **Task Status**: Completed ✅
  -------------------------------------------------------------------------------------

```

#### 三、 Project Main Function Description

##### 1. Project Main Function Description and Gameplay

```markdown
- **This is a simple memory card pairing game, a pure frontend project with no backend dependency, and it can be directly run in a browser. Gameplay and project game main function usage tutorial and explanation**:
### Gameplay
  - The player can freely flip cards to find pairs with the same image. Each time, two cards are flipped. If the two cards match, they remain flipped, and the already flipped cards cannot be flipped back; if they do not match, they return to their original state. The player needs to remember the positions and images of the cards. When all pairs are found, the game ends, i.e., the level is successfully completed.
### Game Main Function Usage Tutorial and Explanation
1. **Game Interface Display**:
   - The game interface consists of a 4×3 grid, totaling 12 cards, with pairs having the same image.
   - Upon starting each game, the card positions are randomly arranged.
2. **Card Pairing Logic**:
   - The player can flip any card to view the image.
   - A maximum of two cards can be flipped per round, with a maximum of one card flipped at a time.
   - If two cards have the same image, they remain flipped and cannot be flipped back; if not, they return to their original state.
   - The game ends when all cards are successfully paired.
3. **Game Reset Functionality**:
   - When refreshing, i.e., each time the game is restarted, the card positions are randomly arranged.
```

##### 2. Project Framework Main Function Description

```markdown
cards-memory-game/              # Project Name: Card Memory Game
├── .git/                          # Git version control-related files, used for managing code versions
├── docs/                          # Project documents
│   └── ...                        # Stores project design documents, usage instructions, etc.
├── gameBase/                      # Game core logic code
│   └── ...                        # Includes game state management, card pairing logic, etc.
├── img/                           # Image resources
│   └── ...                        # Stores all image resources used in the game, including the front and back patterns of the cards
├── NON_CODE_CONTRIBUTIONS/        # Non-code contribution-related content
│   └── ...                        # Such as designs, documents, etc.
├── React/                         # React-related code (if the project is built using React)
│   └── ...                        # Stores React-related components and logic
├── Svelte/                        # Svelte-related code (if the project is built using Svelte)
│   └── ...                        # Stores Svelte-related components and logic
├── translation/                   # Multilingual support files
│   └── ...                        # Stores files for multilingual support, facilitating the game's support for multiple languages
├── TypeScript/                    # TypeScript code (if the project is written in TypeScript)
│   └── ...                        # Stores TypeScript code
├── VUE/                           # Vue-related code (if the project is built using Vue)
│   └── ...                        # Stores Vue-related components and logic
├── .gitignore                     # Git ignore file configuration
│   └── ...                        # Specifies which files are not to be version-controlled
├── CODE_OF_CONDUCT.md             # Project code of conduct
├── CONTRIBUTING.md                # Contribution guidelines
├── LICENSE                        # Open-source license file
├── README.md                      # Project self-explanatory file
│   └── ...                        # Includes project introduction, installation, and usage instructions, etc.
   1. Version Control Management:
   - Use Git for code version control to ensure the history and collaborative development of the code. Configure Git to ignore certain files that do not require version control.
   - docs/: Stores various project documents, including design documents, usage instructions, architecture diagrams, etc., to help developers understand and use the project.
   - README.md: The project's self-explanatory file, providing an introduction to the project, installation, and usage instructions.
   - CODE_OF_CONDUCT.md: The project's code of conduct, regulating the behavior of contributors.
   - CONTRIBUTING.md: Contribution guidelines, explaining how to contribute to the project.
   2. Game Core Logic
   - gameBase/: Stores the core logic code of the game, including game state management, card pairing logic, etc.
   - Game State Management: Manages different states of the game, such as initialization, in-progress, and end.
   - Card Pairing Logic: Implements the core algorithms and rules for card pairing.
   3. Image Resource Management
   - img/: Stores all image resources used in the game, including the front and back patterns of the cards.
   - Non-Code Contributions, Multilingual Support
   - NON_CODE_CONTRIBUTIONS: Stores content related to non-code contributions, such as design drafts, documents, image resources, etc.
   - translation/: Stores files for multilingual support, facilitating the game's support for multiple languages and enhancing its internationalization level.
   4. Frontend Framework Support
   - React, Svelte, VUE: Stores components and logic.
   - TypeScript code, enhancing code maintainability and type safety.
```

##### 3. Screenshot - Project Framework Screenshot

```markdown
![ProjectFramework](D:\2205308010348huangrixin_EnglishFinalExperiment\images\Project Framework. png)
```

##### ![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\ProjectFramework.png)

##### 4.Screenshot - Screenshot of the main functions of the project game interface:

```markdown
![ProjectScreenshot-FeatureImage1Round1](2205308010348huangrixin_EnglishFinalExperiment\images\功能图1-第一轮.png)
```

##### ![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图1-第一轮.png)

```markdown
![ProjectScreenshot-FeatureImage2Round1](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图2-第一轮.png)
```

##### ![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图2-第一轮.png)

```markdown
![ProjectScreenshot-FeatureImage3Round2](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图3-第二轮.png)
```

##### ![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图3-第二轮.png)

```markdown
![ProjectScreenshot-FeatureImage4Round2](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图4-第二轮.png)
```

##### ![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图4-第二轮.png)

```markdown
![ProjectScreenshot-FeatureImage5Round2](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图5-第二轮.png)
```

##### ![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图5-第二轮.png)

```markdown
![ProjectScreenshot-FeatureImage6Round2](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图6-第二轮.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图6-第二轮.png)

```markdown
![ProjectScreenshot-FeatureImage7Round3](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图7-第三轮.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图7-第三轮.png)

```markdown
![ProjectScreenshot-FeatureImage8Round4](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图8-第四轮.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图8-第四轮.png)

```markdown
![ProjectScreenshot-FeatureImage9Round5](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图9-第五轮.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图9-第五轮.png)

```markdown
![ProjectScreenshot-FeatureImage10Round6](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图10-第六轮(闯关成功游戏结束).png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图10-第六轮(闯关成功游戏结束).png)

```markdown
![ProjectScreenshot-FeatureImage11Reopen](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图11-刷新浏览器页面，随机排列.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\功能图11-刷新浏览器页面，随机排列.png)

<!-- by huangrixin -->

## II. ✨Card Memory Game:Part 2 that I am responsible for - TypeScript file description in the project framework

#### 一、Explanation of Group Task Division Selection

```markdown
    <!-- by huangrixin -->
### Explanation: I have chosen Part 5 of the group task. The files included in this part of the project are: MemoryCard.tsx, App.css, main.tsx, and tsconfig.json.
```

##### 1. Screenshot - Original Image of Part 5 Selected in the Group Task

```markdown
![GroupTaskPart5](D:\2205308010348huangrixin_EnglishFinalExperiment\images\huangrixinPart2.png)
```

![](D:\2205308010348huangrixin_EnglishFinalExperiment\images\huangrixinPart2.png)

#### 二、 Tasks-Add tasks and completed tasks

##### 1. Added Tasks and Completed Tasks

```markdown
  1. ✅ Can explain the core gameplay mechanics of the game
  2. ✅ Can describe the CSS implementation principle of card flipping
  3. ✅ Can explain the data flow between components
  4. ✅ Can identify the design approach for state management
  5. ✅ Can recognize the scalability points of the project
  6. ✅ Can explain the performance optimization points
  -  ✅**Conclusion**：Understanding and explanation of the source code for MemoryCard.tsx, App.css, main.tsx, and tsconfig.json files, specifically detailed in -- II. TypeScript Folder Tasks in the Project Framework.
 
```

#### 三、Main Explanation of Source Code Files

##### 1. Core Functionality Understanding and Key Code Analysis

```markdown
## 1. MemoryCard.tsx 
  - **Main Functionality**: The card component responsible for rendering each memory card and handling the card flipping logic.
  - **Code Explanation**: The MemoryCard component receives properties of type MemoryCardProps, including isEnable, handleClick, index, image, name, isDone, and isOpen. The flipCard function handles the card click event, which is only triggered when the card is enabled (isEnable is true). Depending on the isDone and isOpen states, the component decides whether to flip the card. The card consists of two img elements, representing the front and back of the card, respectively.
  - **Key Code**:
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
  - **Main Functionality**: The global style file that defines the overall layout and styling of the application.
  - **Code Explanation**: .memory-game defines the layout of the game container using Flexbox to arrange the cards. .memory-card defines the basic styling of the cards, including size, position, and animation effects. .memory-card.flip defines the styling of the card when it is flipped, achieving the flip effect through transform: rotateY(180deg).
  - **Key Code**:
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
  - **Main Functionality**: Responsible for rendering the React application into the DOM.
  - **Code Explanation**: Uses ReactDOM.createRoot to render the React application into the element obtained by document.getElementById('root'). <React.StrictMode> is used to enable React's strict mode, helping to identify potential issues. <App /> is the root component of the application.
  - **Key Code**:
ReactDOM.createRoot(document.getElementById('root') as HTMLElement).render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);
  -------------------------------------------------------------------------------------
## 4. tsconfig.json 
  - **Main Functionality**: Configures the options for the TypeScript compiler.
  - **Code Explanation**: "target": "ESNext" specifies that TypeScript should compile to the latest JavaScript features. "strict": true enables strict mode, helping to catch common programming errors. "jsx": "react-jsx" specifies the use of React's JSX transformation. "include": ["src"] specifies the source file directory to be included in the compilation.
  - **Key Code**:
{
  "compilerOptions": {
    "jsx": "react-jsx",
    "strict": true,
    "moduleResolution": "Node"
  }
}
```

##### 2. Key Algorithms and Data Structures

```markdown
  - **Algorithm**: Card matching algorithm.
  - **Code**:
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

##### 3. State Management Process

```markdown
### State Management Process
1. Initial Card State: Face down (displaying the JavaScript icon)
2. User clicks → triggers 'flipCard' → calls the parent component's 'handleClick'.
3. Determines whether to display the front image based on the 'isOpen' state.
4. After successful matching, 'isDone' becomes true, keeping the front image displayed.
```

##### 4. Project Scalability

```markdown
### Project Scalability
  - Multi-framework Support: The project structure has been prepared for different implementations such as React/Svelte/Vue.
  - Internationalization Support: A translation directory exists for multi-language support.
  - Resource Management: The img directory centrally manages all card images.
```

##### 5. Project Significance

```markdown
### Project Significance
1. TypeScript Strong Typing: Clearly defines component types.
2. Educational Value: Suitable for front-end teaching and beginners in front-end development.
3. Design Pattern Practice: Demonstrates component communication and state management.
4. Cross-platform Potential: The project structure supports expansion to Web/Mobile.
```

##### 6. Performance Optimization Points

```markdown
### Performance Optimization Points
  - Hardware Acceleration: GPU acceleration is triggered through the transform property.
  - Memory Optimization: Functional components are used to reduce instance overhead.
  - Animation Performance: CSS transitions are superior to JavaScript animations.
```

<!-- by huangrixin -->