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

/* Align form fields in a clean grid */
.block label {
  display: inline-block;
  width: 180px;              /* label width */
  font-weight: bold;
  margin-top: 10px;
  vertical-align: middle;
}

.block input,
.block select,
.block textarea {
  display: inline-block;
  width: 300px;              /* input box width */
  padding: 6px;
  border-radius: 5px;
  border: 1px solid #ccc;
  margin-top: 10px;
  vertical-align: middle;
}

/* For warning text (keeps alignment consistent) */
.warning {
  display: inline-block;
  color: red;
  font-size: 0.9em;
  margin-left: 10px;
  width: 220px;              /* fixed width to prevent layout jumping */
  vertical-align: middle;
}

/* For fieldsets */
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
  width: 300px;
  margin-top: 10px;
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
  margin-right: 10px;
  margin-top: 20px;
}

button:hover {
  background-color: #0056b3;
}

/* Responsive tweak */
@media (max-width: 700px) {
  .block label, 
  .block input, 
  .block select, 
  .block textarea, 
  .warning {
    display: block;
    width: 100%;
  }

  .warning {
    margin-left: 0;
    margin-bottom: 10px;
  }
}

