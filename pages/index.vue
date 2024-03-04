<template>
  <div>
    <header>
      <h1>Welcome to ProjectHub</h1>
      <p>Where projects come to life</p>
      <button class="header-button" @click="navigateToGetStarted">Get Started</button>
    </header>

    <section class="comment-section grow-on-hover">
      <h2>Why Choose ProjectHub?</h2>
      <p class="feature-description">
        ProjectHub integrates Git's robust version control with an intuitive command-line interface, facilitating rapid collaboration and efficient project management.
      </p>
    </section>

    <section class="comment-section grow-on-hover">
      <h2>Effortless Collaboration</h2>
      <p class="feature-description">
        Simplify your team's workflow with ProjectHub. Our platform streamlines project management and change tracking, allowing for seamless collaboration.
      </p>
    </section>

    <section class="comment-section grow-on-hover">
      <h2>Cross-Platform Support</h2>
      <p class="feature-description">
        Utilizing Electron, ProjectHub offers a versatile desktop environment across multiple operating systems. Though Electron is known for its resource intensity, we're committed to optimizing performance for a smoother experience.
      </p>
    </section>

    <section class="comment-section grow-on-hover">
      <h2>Real-Time Updates</h2>
      <p class="feature-description">
        Keep your team in sync with live notifications and updates. ProjectHub's real-time updates ensure that everyone stays informed and aligned on project progress.
      </p>
    </section>

    <section class="comment-section grow-on-hover">
      <h2>Secure and Reliable</h2>
      <p class="feature-description">
        At ProjectHub, we prioritize your security. With end-to-end encryption, consistent backups, and dependable uptime, you can trust that your data is safe with us.
      </p>
    </section>

    <footer>
      <p>&copy; 2024 ProjectHub. All rights reserved.</p>
    </footer>
  </div>
</template>

<script>
export default {
  methods: {
    navigateToGetStarted() {
      this.$router.push('/app');
    },
  },
};
</script>

<style scoped>
div {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background-color: #121212; /* Darker shade for background */
  color: #ececec; /* Light color for text for contrast */
  min-height: 100vh; /* Ensure div covers the whole viewport height */
  display: flex;
  flex-direction: column;
  align-items: center; /* Center content horizontally */
}

header {
  text-align: center;
  padding: 60px 20px; /* Add some padding for spacing */
}

.header-button {
  background-color: #2ecc71; /* Dark green color for the button */
  color: white; /* White text color for the button */
  border: none; /* Remove default border */
  padding: 12px 24px; /* Increased padding for better clickability */
  font-family: 'Arial', 'Helvetica', sans-serif;
  font-size: 18px; /* Larger font size for emphasis */
  cursor: pointer; /* Change cursor to pointer on hover */
  border-radius: 8px; /* Rounder corners for the button */
  transition: background-color 0.3s; /* Smooth transition for button hover */
  margin-top: 20px; /* Add some space above the button */
}

.header-button:hover {
  background-color: #27ae60; /* Slightly lighter shade on hover */
}

.comment-section {
  background-color: #1e1e1e; /* Darker color for comment sections */
  border-radius: 8px; /* Rounded corners for comment sections */
  margin: 20px 0; /* Add some margin between comment sections */
  padding: 20px; /* Adjusted padding for better sizing */
  width: 80%; /* Limit section width */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Add subtle box shadow */
}

.grow-on-hover {
  transition: transform 0.3s; /* Smooth transition for growth effect */
}

.grow-on-hover:hover {
  transform: scale(1.05); /* Grow by 5% on hover */
}

h2 {
  color: #2ecc71; /* Match the button color for consistency */
  margin-bottom: 10px; /* Add some space below the heading */
}

.feature-description {
  max-width: 600px; /* Limit the width for better readability */
  text-align: center;
  line-height: 1.6; /* Improved line height for better legibility */
  margin: auto; /* Center the text block */
}

footer {
  background-color: #1e1e1e; /* Darker color for footer */
  text-align: center;
  padding: 20px 0;
  color: #ececec; /* Light color for text for contrast */
  width: 100%; /* Ensure footer spans the width of the page */
}
</style>
