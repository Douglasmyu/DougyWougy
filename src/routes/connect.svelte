<section>
    <div class="contact-form">
      <!-- <h2>Contact Me</h2>
      <input type="email" bind:value={email} placeholder="Your Email" required />
      <input type="text" bind:value={subject} placeholder="Subject" required />
      <textarea bind:value={message} placeholder="Your Message" rows="4" required></textarea>
      <button on:click={sendEmail}>Send Email</button> -->
    </div>
  </section>
  <section class = "container"> <!--Links section-->
    <p class="title">
      Connect with me!
    </p>
    <!-- <button class="Coolbutton" on:click={openGithub}>github</button> -->
    <img src="/img/gitIcon.png" class="icon" on:click={openGithub}>
    <img src="/img/linkedInIcon.png" class="icon "on:click={openLinkedIn}>
    <img src="/img/spotifyIcon.png" class="icon" on:click={openSpotify}>
  </section>
  <script>
    function openLinkedIn(){
      window.open('https://www.linkedin.com/in/douglas-yu-51614b165/');
    }
    function openGithub() {
      window.open('https://github.com/Douglasmyu');
    }
    function openSpotify(){
      window.open('https://open.spotify.com/user/douglife-us?si=e9b2a5f65a064dcc');
    }
  </script>

<style>
    .container {
      display: flex;
		  flex-direction: column;
		  justify-content: center;
		  align-items: center;
		  width: 100%;
		  margin: 0 auto;
      background-color: #f2eee2;
    }
    .title {
        color:#963b44;
        font-size: medium;
        text-align: center;
    }

    .icon{
    cursor: pointer;
    }

    .icon:hover{
    opacity: 0.8;
    }

</style>