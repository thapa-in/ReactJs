Navbar code in original React Code

Three things to Understand
1. import react-router-dom is file helps us to create / operate links for open pages
2. index.js : Wrap up the <App/> with <BrowserRouter> for support Router, Links
3. App.js : In <App/> we have to create Routes link.
4. Navbar.js : Make links in a component file or in view page component

Step By Step
1. Wrap up the <App/> tag with <BrowserRouter>
```
<BrowserRouter>
   <App />
</BrowserRouter>
```
2. Make Routes in App.js file
```
import logo from './logo.svg';
import './App.css';
import Home from './Home';
import About from './About';
import { Route, Routes } from 'react-router-dom';

function App() {
  return (
    <>
      <Routes>
        <Route path="/Home" element={<Home />} />
        <Route path="/About" element={<About />} />
      </Routes>
    </>
  );
}

export default App;
```
3. Make component in components folder
```
import React from 'react';
import { Link } from 'react-router-dom';

const Navbar = () => {
    return (
        <>
        <Link to="/">Home</Link>
            <ul>
                <li>
                    <Link to="/About">DashBoard</Link>
                </li>
            </ul>
        </>
    )
}
export default Navbar
```
