<section class = "container">
    <div class = "content">
        <h1 class = "title">About Me</h1>
            <p class="description">
                Hi I'm Douglas.  I am currently a Computer Science student at Cal State Fullerton. 
                I enjoy coding, learning new things, and having fun!
                When I am not coding, I am probably cooking, trying out new cafes, 
                designing and sewing my own clothes, gyming, golfing, or playing badminton.
                <!--gonna need to change when I graduate-->
            </p>
            <div class = "resume">
                <a href="Douglas-5.pdf">Resume</a> <!--make icon-->
                <img alt ="resume" src="/img/resumeIcon.png">
            </div>
    </div>
</section>
<script>
    import Toggle from './Toggle.svelte';
</script>
<style>
    .container {
        display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		width: 100%;
		height: 100vh;
		margin: 0 auto;
        background-color: #f2eee2;
    }
    .title {
        font-size: larger;
        margin: 0 auto;
        justify-content: center;
        flex-direction: column;
        align-items: center;
        margin: 0 auto;
        display: flex;
        color: rgba(255, 109, 109, 0.8);
    }
    .description {
        font-size: 18px;
        color:#0084f6;
        width: 50%;
        justify-content: center;
        flex-direction: column;
        align-items: center;
        margin: 0 auto;
        display: flex;
    }
    .resume {
		display: block;
		text-decoration: none;
		color: white;
		padding: 0.5rem 1rem;
        justify-content: center;
        flex-direction: column;
        align-items: center;
        margin: 0 auto;
        display: flex;
	}
    @media (max-width: 768px) {
		.container {
			width: 80%;
		}
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