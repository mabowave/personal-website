<script>
  let interests = ['Programming', 'Cheese', 'Golf'];
</script>
<h1>This is my website!</h1>
<main class="container">
  <h1>Hello, I'm <span class="highlight">Mason Fu</span>!</h1>

  <section class="card">
    <h2>About Me</h2>
    <p>
      I like programming, cheese, and playing golf.
    </p>
    <p>I program in a little html, mostly python, and a little css.</p>
    <p>My favorite types of cheese are parmesan, sharp cheddar, and mozzarella.</p>
    <p>In golf, I mostly play for fun.</p>
    <p>I got a riddle for you. 1. A man rides in on Friday, and 3 days later leaves on Friday. How is this possible?</p>
    <p>I have some others too. 2. What has keys but does not open any doors?</p>
    <p>3.What kind of room cannot be opened?</p>
    <p><b>The answers are at the bottom.</b></p>
    <button>Here is something you can click for fun.</button>
  </section>

  <section class="card">
    <h2>My Interests</h2>
    <ul class="interests">
      {#each interests as interest}
        <li>{interest}</li>
      {/each}
    </ul>
    <p>1. The horse is named Friday. 2. A keyboard. 3. a mushroom.</p>
  </section>
</main>

<style>
  body {
    margin: 0;
    background: linear-gradient(135deg, #ffe5b4, #ffd2a6, #ffb385);
    font-family: 'Poppins', system-ui, sans-serif;
    color: #4a2c1f;
    background-attachment: fixed;
  }

  .container {
    max-width: 700px;
    margin: 5rem auto;
    padding: 2rem;
    text-align: center;
  }

  h1 {
    font-size: 3.5rem;
    margin-bottom: 0.5rem;
  }

  .highlight {
    color: #e07a5f; /* warm terracotta color */
  }

  .subtitle {
    font-size: 1.2rem;
    color: #7b3e19;
    margin-bottom: 3rem;
  }

  h2 {
    font-size: 2rem;
    margin-bottom: 1rem;
    color: #d65a31;
  }

  .card {
    background: #fffaf0;
    padding: 2rem;
    margin-bottom: 2rem;
    border-radius: 16px;
    box-shadow: 0 6px 14px rgba(0, 0, 0, 0.08);
  }

  ul.interests {
    list-style: none;
    padding: 0;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1rem;
  }

  ul.interests li {
    background: #ff7f50;
    color: white;
    padding: 0.5rem 1.2rem;
    border-radius: 20px;
    font-size: 1rem;
    transition: background 0.3s ease;
    cursor: pointer;
  }

  ul.interests li:hover {
    background: #ff5722;
  }
</style>
