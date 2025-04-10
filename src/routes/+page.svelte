<script>
  const slackId = "U12345678"; // TODO: Replace with your actual Slack ID!
</script>

<div class="app-container">
  <a href="https://hackclub.com/">
    <img
      style="position: absolute; top: 0; left: 50px; border: 0; width: 128px; z-index: 999;"
      src="https://assets.hackclub.com/flag-orpheus-top.svg"
      alt="Hack Club"
    />
  </a>

  <div class="content">
    <h1>Welcome to my Hack Club Site!</h1>
    <p>Created by {slackId}</p>
  </div>
</div>

<style>
  :root {
    --red: #ec3750;
    --orange: #ff8c37;
    --yellow: #f1c40f;
    --green: #33d6a6;
    --cyan: #5bc0de;
    --blue: #338eda;
    --purple: #a633d6;
    --muted: #8492a6;
  }

  @font-face {
    font-family: "Phantom Sans";
    src:
      url("https://assets.hackclub.com/fonts/Phantom_Sans_0.7/Regular.woff") format("woff"),
      url("https://assets.hackclub.com/fonts/Phantom_Sans_0.7/Regular.woff2") format("woff2");
    font-weight: normal;
    font-style: normal;
    font-display: swap;
  }

  @font-face {
    font-family: "Phantom Sans";
    src:
      url("https://assets.hackclub.com/fonts/Phantom_Sans_0.7/Italic.woff") format("woff"),
      url("https://assets.hackclub.com/fonts/Phantom_Sans_0.7/Italic.woff2") format("woff2");
    font-weight: normal;
    font-style: italic;
    font-display: swap;
  }

  @font-face {
    font-family: "Phantom Sans";
    src:
      url("https://assets.hackclub.com/fonts/Phantom_Sans_0.7/Bold.woff") format("woff"),
      url("https://assets.hackclub.com/fonts/Phantom_Sans_0.7/Bold.woff2") format("woff2");
    font-weight: bold;
    font-style: normal;
    font-display: swap;
  }

  :global(body) {
    margin: 0;
    padding: 0;
    font-family:
      "Phantom Sans",
      -apple-system,
      BlinkMacSystemFont,
      "Segoe UI",
      "Roboto",
      "Oxygen",
      "Ubuntu",
      "Cantarell",
      "Fira Sans",
      "Droid Sans",
      "Helvetica Neue",
      sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }

  :global(html, body) {
    width: 100%;
    height: 100%;
  }

  .app-container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: white;
  }

  .content {
    margin-top: 60px;
    text-align: center;
    padding: 2rem;
  }

  h1 {
    color: var(--red);
    margin-bottom: 1rem;
    font-size: 4rem;
  }

  @media (max-width: 768px) {
    h1 {
      font-size: 2rem;
    }
  }

  p {
    color: var(--muted);
    font-size: 1.2rem;
  }

  @keyframes orpheus-flag {
    0% {
      transform: rotate(0deg);
    }

    100% {
      transform: rotate(-5deg);
    }
  }

  @media (prefers-reduced-motion: no-preference) {
    img {
      transform-origin: left top;
      animation: 0.5s linear 0s infinite alternate none running orpheus-flag;
    }
  }
</style>