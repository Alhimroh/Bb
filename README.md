`javascript
// Mendefinisikan variabel-variabel yang diperlukan
var username = "pengguna";
var password = "sandi";
var baseURL = "https://domain-anda.com/login";

// Membuat URL login dengan menggunakan variabel-variabel yang telah didefinisikan
var loginURL = `${baseURL}?username=${username}&password=${password}`;

// Output URL login
console.log(loginURL);
