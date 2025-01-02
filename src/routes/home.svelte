<script>
     import Toggle from './Toggle.svelte';
</script>
<section>
    <div class="navbar">
        <div class = "navbar-left">
            <img src= "/img/pfp.jpg" alt="pfp">
            <center><p class="name"><b>douglas yu</b></p></center>
            <a href="#about">About Me</a>
            <a href="#projects">Projects</a>
            <a href="#skills">Skills</a>
            <a href="#hobbies">Hobbies</a>
            <!-- <Toggle/> -->
        </div>
      </div>
</section>

<style>
     .navbar {
      display: flex;
      justify-content: space-around;
      align-items: center;
      background-color: #444;
      padding: 1rem;
    }
    .navbar-left {
        align-items: center;
        display: flex;
        gap: 1rem;
    }
    .navbar img {
        width: 70px;
        height: 70px;
        border-radius: 50%;
        object-fit: cover; 
        margin-right: 1rem;
    }
    :global(body) {
        background-color: #f2eee2;
        color: #0084f6;
        transition: background-color 0.3s;
    }

    :global(body.dark-mode) {
        background-color: #1d3040;
        color: #bfc2c7;
    }
</style>