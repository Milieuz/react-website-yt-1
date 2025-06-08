# React Beginner Project
Evan Wheeler - 6/7/2025

* Run with 'npm start' inside of root folder.

Ported from this YT Video:<br>
https://www.youtube.com/watch?v=I2UBjN5ER4s<br>
And this repo:<br>
https://github.com/briancodex/react-website-v1/tree/starter<br>

Had to update for newer React version via the following:<br>
## (1)
"Switch" is now Routes (in App.js):<br>
import { BrowserRouter as Router, Routes, Route } from 'react-router-dom';<br>

## (2)
Source the above change appropriately in App.js links:<br>

    <>

      <Router>

        <Navbar />

        <Routes>

          <Route path="/" exact element={<Home />} />

          <Route path="/services" element={<Services />} />

          <Route path="/products" element={<Products />} />

          <Route path="/sign-up" element={<SignUp />} />

        </Routes>

      </Router>

    </>

## (3)
Update the relative image links in App.css to add '../public', i.e.<br>

../public/images/img-2.jpg<br>
../public/images/img-1.jpg<br>
../public/images/img-8.jpg<br>

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).