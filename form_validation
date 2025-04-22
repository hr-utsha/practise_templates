```
<!DOCTYPE html>
<html>
<head>
  <title>Advanced Form Validation</title>
  <style>
    .error {
      color: red;
      font-size: 12px;
    }

    .input-error {
      border: 2px solid red;
    }
  </style>
</head>
<body>

<h2>Registration Form</h2>

<form id="myForm">
  <label>Name:</label>
  <input type="text" id="name">
  <span class="error" id="nameError"></span><br><br>

  <label>Email:</label>
  <input type="text" id="email">
  <span class="error" id="emailError"></span><br><br>

  <label>Password:</label>
  <input type="password" id="password">
  <span class="error" id="passwordError"></span><br><br>

  <button type="button" onclick="validateForm()">Submit</button>
</form>

<script>
  function validateForm() {
    // Clear previous error messages and styles
    document.getElementById("nameError").innerText = "";
    document.getElementById("emailError").innerText = "";
    document.getElementById("passwordError").innerText = "";

    document.getElementById("name").classList.remove("input-error");
    document.getElementById("email").classList.remove("input-error");
    document.getElementById("password").classList.remove("input-error");

    let name = document.getElementById("name").value.trim();
    let email = document.getElementById("email").value.trim();
    let password = document.getElementById("password").value;

    let isValid = true;

    // Name Validation
    if (name.length < 3) {
      document.getElementById("nameError").innerText = "নাম কমপক্ষে ৩ অক্ষরের হতে হবে";
      document.getElementById("name").classList.add("input-error");
      isValid = false;
    }

    // Email Validation (using regex)
    let emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;  // let emailPattern = /^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$/;
    

    if (!emailPattern.test(email)) {
      document.getElementById("emailError").innerText = "সঠিক ফরম্যাটে ইমেইল দিন (উদাহরণ: example@mail.com)";
      document.getElementById("email").classList.add("input-error");
      isValid = false;
    }

    // Password Validation
    let passwordPattern = /^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[!@#$%^&*]).{8,}$/;
    if (!passwordPattern.test(password)) {
      document.getElementById("passwordError").innerText = "পাসওয়ার্ডে অন্তত ৮ অক্ষর, ১টি বড় ও ছোট হাতের অক্ষর, ১টি সংখ্যা এবং ১টি special character থাকতে হবে";
      document.getElementById("password").classList.add("input-error");
      isValid = false;
    }

    // Final result
    if (isValid) {
      alert("Form Submitted Successfully!");
    }
  }
</script>

</body>
</html>

```
