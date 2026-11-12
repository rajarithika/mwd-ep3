# Exp 03 – React Lab Exercise: State in React using useState()

## **NAME : Raja Rithika**

## **REG NO: 2305001029**

---

## Aim

To create a React application that demonstrates the use of State using the useState() Hook and understand how state changes update the user interface.

## Objectives

- To understand the concept of State in React.
- To create state variables using the useState() Hook.
- To update state using state setter functions.
- To handle button click events using onClick.
- To understand how changing state causes the component to re-render.
- To implement counter, student name, department, like button, and attendance applications.

## Program

### Step 1: Create a React Project

```bash
npm create vite@latest state-demo
cd state-demo
npm install
npm run dev
```

### Step 2: App.jsx

Open `src/App.jsx` and paste the following code:

```jsx
import { useState } from "react";

function App() {

  // Counter State
  const [count, setCount] = useState(0);

  // Student Name State
  const [name, setName] = useState("admin");

  // Department State
  const [department, setDepartment] = useState("CSE");

  // Like Button State
  const [likes, setLikes] = useState(0);

  // Student Attendance State
  const [attendance, setAttendance] = useState(0);

  return (
    <div>

      <h1>React State Example</h1>

      <hr />

      {/* Student Name */}
      <h2>Student Name: {name}</h2>

      <button onClick={() => setName("Raja Rithika")}>
        Change Name
      </button>

      <hr />

      {/* Counter */}
      <h2>Count: {count}</h2>

      <button onClick={() => setCount(count + 1)}>
        Increase
      </button>

      <button onClick={() => setCount(count - 1)}>
        Decrease
      </button>

      {/* Reset Counter */}
      <button onClick={() => setCount(0)}>
        Reset
      </button>

      <hr />

      {/* Student Department */}
      <h2>Department: {department}</h2>

      <button onClick={() => setDepartment("ECE")}>
        Change Department
      </button>

      <hr />

      {/* Like Button */}
      <h2>Likes: {likes}</h2>

      <button onClick={() => setLikes(likes + 1)}>
        Like
      </button>

      <hr />

      {/* Student Attendance */}
      <h2>Student Attendance</h2>

      <h3>Present: {attendance}</h3>

      <button onClick={() => setAttendance(attendance + 1)}>
        Present
      </button>

      <button onClick={() => setAttendance(Math.max(0, attendance - 1))}>
        Absent
      </button>

      <button onClick={() => setAttendance(0)}>
        Reset Attendance
      </button>

    </div>
  );
}

export default App;
```

### Step 3: index.css

Open `src/index.css` and paste:

```css
body {
  font-family: Arial, sans-serif;
  text-align: center;
  margin-top: 50px;
  background-color: #f5f5f5;
}

h1 {
  color: black;
}

h2 {
  color: black;
}

button {
  padding: 10px 20px;
  margin: 5px;
  font-size: 16px;
  cursor: pointer;
}
```

## Output
<img width="1306" height="1205" alt="image" src="https://github.com/user-attachments/assets/9041cbf3-440f-4533-a43e-4be414345705" />


## Result

Thus, a React application was successfully created and executed using the useState() Hook to demonstrate state management, button click events, and dynamic user interface updates through counter, student name, department, like button, and attendance activities.
