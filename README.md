/* General layout */
body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f9;
  margin: 40px;
}

h1 {
  text-align: center;
  color: #333;
  margin-bottom: 30px;
}

.block {
  background-color: #fff;
  border-radius: 10px;
  box-shadow: 0 0 8px rgba(0,0,0,0.1);
  padding: 20px 30px;
  margin-bottom: 25px;
}

/* Form field grid for perfect alignment */
.block form {
  display: grid;
  grid-template-columns: 180px 300px 220px; /* label | input | warning */
  align-items: center;
  row-gap: 12px;
  column-gap: 10px;
}

/* Label styling */
.block label {
  font-weight: bold;
  text-align: right;
}

/* Inputs, selects, and textareas */
.block input,
.block select,
.block textarea {
  width: 100%;
  padding: 6px;
  border-radius: 5px;
  border: 1px solid #ccc;
  box-sizing: border-box;
}

/* Warning messages stay in the same column for alignment */
.warning {
  color: red;
  font-size: 0.9em;
}

/* Fieldsets */
fieldset {
  border: 1px solid #ccc;
  border-radius: 8px;
  margin-top: 15px;
  padding: 10px 15px;
}

fieldset legend {
  font-weight: bold;
}

/* Range slider and value alignment */
#salary {
  width: 100%;
}

#salaryValue {
  font-weight: bold;
  margin-left: 10px;
}

/* Buttons */
button {
  background-color: #007bff;
  color: white;
  border: none;
  padding: 10px 20px;
  border-radius: 8px;
  cursor: pointer;
  font-size: 1em;
  margin-top: 20px;
}

button:hover {
  background-color: #0056b3;
}

/* Responsive layout */
@media (max-width: 700px) {
  .block form {
    grid-template-columns: 1fr;
  }

  .block label {
    text-align: left;
  }

  .warning {
    margin-top: -5px;
  }
}

