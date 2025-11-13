<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Homework 3 – New User Form</title>
  <link rel="stylesheet" href="style.css">
  <script defer src="script.js"></script>
</head>

<body>
  <h1>New User Form</h1>

  <form id="userForm" novalidate>
    <div class="block">
      <h2>Personal Information</h2>

      <label for="firstName">First Name</label>
      <input type="text" id="firstName" name="firstName" title="1–30 letters, apostrophes, or dashes only" />
      <span class="warning" id="firstNameWarn"></span>

      <label for="middleInitial">Middle Initial</label>
      <input type="text" id="middleInitial" name="middleInitial" title="Optional, 1 letter only" />
      <span class="warning" id="middleInitialWarn"></span>

      <label for="lastName">Last Name</label>
      <input type="text" id="lastName" name="lastName" title="1–30 letters, apostrophes, or dashes only" />
      <span class="warning" id="lastNameWarn"></span>

      <label for="birthDate">Date of Birth</label>
      <input type="date" id="birthDate" name="birthDate" title="Must be a valid date, not future or older than 120 years" />
      <span class="warning" id="birthDateWarn"></span>

      <label for="idNumber">ID Number (9 digits)</label>
      <input type="password" id="idNumber" name="idNumber" maxlength="11" title="9 digits, dashes auto-added" />
      <span class="warning" id="idNumberWarn"></span>
    </div>

    <div class="block">
      <h2>Address Information</h2>

      <label for="address1">Address Line 1</label>
      <input type="text" id="address1" name="address1" title="2–30 characters required" />
      <span class="warning" id="address1Warn"></span>

      <label for="address2">Address Line 2</label>
      <input type="text" id="address2" name="address2" title="Optional, 2–30 characters" />
      <span class="warning" id="address2Warn"></span>

      <label for="city">City</label>
      <input type="text" id="city" name="city" title="2–30 letters only" />
      <span class="warning" id="cityWarn"></span>

      <label for="state">State</label>
      <select id="state" name="state">
        <option value="">-- Select State --</option>
        <option>AL</option><option>AK</option><option>AZ</option><option>AR</option>
        <option>CA</option><option>CO</option><option>CT</option><option>DE</option>
        <option>DC</option><option>FL</option><option>GA</option><option>HI</option>
        <option>ID</option><option>IL</option><option>IN</option><option>IA</option>
        <option>KS</option><option>KY</option><option>LA</option><option>ME</option>
        <option>MD</option><option>MA</option><option>MI</option><option>MN</option>
        <option>MS</option><option>MO</option><option>MT</option><option>NE</option>
        <option>NV</option><option>NH</option><option>NJ</option><option>NM</option>
        <option>NY</option><option>NC</option><option>ND</option><option>OH</option>
        <option>OK</option><option>OR</option><option>PA</option><option>PR</option>
        <option>RI</option><option>SC</option><option>SD</option><option>TN</option>
        <option>TX</option><option>UT</option><option>VT</option><option>VA</option>
        <option>WA</option><option>WV</option><option>WI</option><option>WY</option>
      </select>
      <span class="warning" id="stateWarn"></span>

      <label for="zip">Zip Code</label>
      <input type="text" id="zip" name="zip" maxlength="5" title="5 digits only" />
      <span class="warning" id="zipWarn"></span>
    </div>

    <div class="block">
      <h2>Contact</h2>

      <label for="email">Email</label>
      <input type="email" id="email" name="email" title="Format: name@domain.com" />
      <span class="warning" id="emailWarn"></span>
    </div>

    <div class="block">
      <h2>Preferences</h2>

      <fieldset>
        <legend>Check all that apply:</legend>
        <label><input type="checkbox" name="disease" value="chickenpox"> Chicken Pox</label>
        <label><input type="checkbox" name="disease" value="measles"> Measles</label>
        <label><input type="checkbox" name="disease" value="covid"> Covid-19</label>
        <label><input type="checkbox" name="disease" value="flu"> Flu</label>
        <label><input type="checkbox" name="disease" value="other"> Other</label>
      </fieldset>

      <fieldset>
        <legend>Do you own or rent?</legend>
        <label><input type="radio" name="housing" value="own"> Own</label>
        <label><input type="radio" name="housing" value="rent"> Rent</label>
        <label><input type="radio" name="housing" value="unsure"> Unsure</label>
      </fieldset>

      <label for="salary">Desired Salary</label>
      <input type="range" id="salary" min="20000" max="200000" step="1000" value="60000">
      <span id="salaryValue">$60,000</span>

      <label for="comments">Comments</label>
      <textarea id="comments" name="comments" rows="3" cols="40"></textarea>
    </div>

    <div class="block">
      <h2>Account Setup</h2>

      <label for="userID">Desired User ID</label>
      <input type="text" id="userID" name="userID" title="5–20 chars, start with letter, letters/numbers/_/- only" />
      <span class="warning" id="userIDWarn"></span>

      <label for="password">Password</label>
      <input type="password" id="password" name="password" title="8–30 chars, include upper, lower, number" />
      <span class="warning" id="passwordWarn"></span>

      <label for="confirmPassword">Re-enter Password</label>
      <input type="password" id="confirmPassword" name="confirmPassword" />
      <span class="warning" id="confirmPasswordWarn"></span>
    </div>

    <button type="button" id="validateBtn">Validate</button>
    <button type="submit" id="submitBtn" disabled>Submit</button>
  </form>
</body>
</html>
