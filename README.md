function login() {
  var username = document.getElementById("username").value;
  var password = document.getElementById("password").value;

  // Mock authentication, replace with actual logic on the server
  if (username === "user" && password === "pass") {
    // Redirect to a specific URL after successful login
    window.location.href = "https://example.com/dashboard";
  } else {
    alert("Login failed. Please check your credentials.");
  }
}
// Ganti example.com dengan domain sesuai proyek Anda
window.location.href = "https://domain-anda.com/dashboard";
