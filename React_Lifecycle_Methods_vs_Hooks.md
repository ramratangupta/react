#Gemini promt - list all react equivalent life cycle methods for class and function component and present in to col view md parsed

| Class Component Lifecycle Methods | Functional Component Hooks (Equivalents) |
|---|---|
| `constructor(props)` | `useState` (initial state), outside the component (initial setup) |
| `componentDidMount()` | `useEffect` (with empty dependency array `[]`) |
| `componentDidUpdate(prevProps, prevState)` | `useEffect` (with dependency array containing props or state variables) |
| `componentWillUnmount()` | `useEffect` (return cleanup function) |
| `shouldComponentUpdate(nextProps, nextState)` | `React.memo`, `useMemo`, `useCallback` (for performance optimizations) |
| `getDerivedStateFromProps(nextProps, prevState)` | `useState` (with a function as initial state), `useMemo` |
| `getSnapshotBeforeUpdate(prevProps, prevState)` | `useRef` (to capture values before DOM updates) |
| `componentDidCatch(error, info)` | `ErrorBoundary` components, or try/catch blocks within the component |