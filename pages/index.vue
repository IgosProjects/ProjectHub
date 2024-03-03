<template>
  <div>
    <header>
      <h1>Welcome to ProjectHub</h1>
      <p>Where programs meet</p>
      <button class="header-button">Get Started</button>
    </header>
  </div>
</template>

<style>
div {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background-color: #2c3e50; /* Darker shade for background */
  color: #ecf0f1; /* Light color for text for contrast */
  min-height: 100vh; /* Ensure div covers the whole viewport height */
}

header {
  text-align: center;
  padding: 60px 20px; /* Add some padding for spacing */
}

.header-button {
  background-color: #42b983; /* Vue.js green color for the button */
  color: white; /* White text color for the button */
  border: none; /* Remove default border */
  padding: 10px 20px; /* Padding inside the button */
  font-family: Arial, Helvetica, sans-serif;
  font-size: 16px; /* Slightly larger font size */
  cursor: pointer; /* Change cursor to pointer on hover */
  border-radius: 5px; /* Slightly round corners for the button */
  transition: background-color 0.3s; /* Smooth transition for button hover */
}

</style>