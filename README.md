# REACT-AddingImages

### In-line styles require quotes around values

import background from './images/background_photo_desktop.jpg;'

const App = () =>{
    return (
        <div style={{ //in-line styles require quotes around values
            backgroundImage: "url(./images/background_photo_desktop.jpg)",
            }}>
        </div>
    )

### Set backgroundImage in REACT with Inline CSS Style and import CSS Style

If you put an image.png file inside the public/ folder, you can access it at <your host address>/image.png.  <br/>
Running React in your local computer, the image should be at http://localhost:3000/image.png.  <br/>

### Using the Relative URL Method
Users can access images from the public/ folder or any child folder of the public folder<br/>
The public/ folder used to add static assets. <br/>
URL to access the image should be like <host_name>/image.png.<br/>

  <div style={{ backgroundImage: "url(/image.png)" }}>
    Hello World
  </div>
  
### Using the Absolute URL Method

Users can access the background image directly from the public/ folder via absolute URL using the environment variable. <br/>
backgroundImage: `url(${
                process.env.PUBLIC_URL + "/image.png"
            })`,
### Add background image from src/ folder in React

//IMPORT From Your /src Folder
import React from 'react';
import './index.css';
import img from './images/check.png';

const App = () =>{
    return (  <div style={ backgroundImage: `url(${background})`},>
                <img
                src={img} 
                />
              </div>
       


