# 2400032379-skill-exam
import React, { useState } from "react";

function ClickEvent() {
  const [message, setMessage] = useState("Click the button!");

  function handleClick() {
    setMessage("Button Clicked!");
    alert("Button was clicked!");
  }

  const buttonStyle = {
    backgroundColor: "lightblue",
    color: "black",
    border: "none",
    padding: "10px 20px",
    fontSize: "16px",
    borderRadius: "8px",
    cursor: "pointer",
  };

  const headingStyle = {
    color: "darkblue",
    fontFamily: "Arial, sans-serif",
  };

  return (
    <div>
      <h2 style={headingStyle}>{message}</h2>
      <button style={buttonStyle} onClick={handleClick}>
        Click Me
      </button>
    </div>
  );
}

export default ClickEvent;
