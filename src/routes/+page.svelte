<script>
    let veganCakeDay = null; // User's vegan start date
  </script>
  
  <main>
    <!-- Global Counter Section -->
    <section id="global-counter" class="section">
      <h2>Global Impact</h2>
      <p>Live counter showing ongoing harm (animals, CO2, water, land, etc.).</p>
      <div class="counter">[Global Counter Placeholder]</div>
    </section>
  
    <!-- Personal Counter Section -->
    <section id="personal-counter" class="section">
      <h2>Your Impact</h2>
      {#if veganCakeDay}
        <p>Since your Vegan Cake Day, you've saved:</p>
        <div class="counter">[Personal Counter Placeholder]</div>
      {:else}
        <p>Choose your Vegan Cake Day to see your impact!</p>
        <button on:click={() => veganCakeDay = new Date()}>Pick Your Vegan Cake Day</button>
      {/if}
    </section>
  
    <!-- Call to Action: Stop the Count -->
    <section id="call-to-action" class="section">
      <h2>Stop the Count</h2>
      <p>Join the movement and stop your personal count.</p>
      <button>I'm Vegan Now!</button>
    </section>
  
    <!-- Share Section -->
    <section id="share" class="section">
      <h2>Share Your Impact</h2>
      <p>Let others know about your decision.</p>
      <button>Share on Social Media</button>
    </section>
  
    <!-- About & Sources Section -->
    <section id="about" class="section">
      <h2>About This Project</h2>
      <p>How we calculate the numbers and where our data comes from.</p>
      <a href="#sources">View Sources</a>
    </section>
  
    <section id="sources" class="section">
      <h2>Data Sources</h2>
      <p>List of reliable sources used for calculations.</p>
    </section>
  </main>
  
  <style>
    .section {
      padding: 2rem;
      border-bottom: 1px solid #ccc;
    }
  </style>
  