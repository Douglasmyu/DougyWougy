<section class = "container">
    <div class = "content">
        <h1 class = "header">PROJECTS</h1>
        <div class = "groups">
            <a href = https://sympto-quest-phi.vercel.app/login class="project-link" target="_blank">
                <div class = "project"> <!--SymptoQuest-->
                    <img src = "symptoQuest.png" alt = "symptoQuest pic">
                    <div class = "description">
                        <h2>SymptoQuest</h2>
                        <p>
                        SymptoQuest is a web application that provides accurate medical diagnosis based on user input symptoms
                        </p>
                    </div>
                </div>
            </a>
               
            <a href = https://github.com/Douglasmyu/Tuffy-Reminder class="project-link" target="_blank">
                <div class = "project"><!--tuffy reminder-->
                    <img src = "tuffyreminder3.png" alt = "tuffyreminder pic">
                    <div class = "description">
                        <h2>Tuffy Reminder</h2>
                        <p>
                        IOS task manager app that lets users create task, set a due date, and time their work, improving effiency
                        </p>
                    </div>
                </div>
            </a>
                
            <a href = https://github.com/chandpranav/WeatherWise class="project-link" target="_blank">
                <div class = "project"><!--weather wise-->
                    <img src = "weatherwise1.png" alt = "weatherwise pic">
                    <div class = "description">
                        <h2>WeatherWise</h2>
                        <p>
                        Web app that lets you search for a city and find an accurate weather report using the api's and shit
                        </p>
                    </div>  
                </div>
            </a>
                
            <a href = https://github.com/Tepah/Project-Nyaan class="project-link" target="_blank">
                <div class = "project"><!--nyaan cat-->
                    <img src = "nyaanPhoto.png" alt = "nyaan cat pic">
                    <div class = "description">
                        <h2>Project Nyaan</h2>
                        <div class="tech-list">
							<p class="tech">Unity</p>
							<p class="tech">JavaScript</p>
							<p class="tech">React</p>
						</div>
                        <!-- <p>
                        Nyaan cat is an astronaut doing a space walk. During his space walk, he sees a bunch of fish falling from the sky!! 
                        Yummers!! Move Nyaan around space to eat as much fish as possible and avoid the bombs or else he will die!! 😱
                        </p> -->
                    </div>     
                </div>
            </a>      
                
        </div>
                
            
    </div>
</section>

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
    .header {
        font-size: larger;
        margin: 0 auto;
        justify-content: center;
        flex-direction: column;
        align-items: center;
        margin: 0 auto;
        display: flex;
        color: rgba(255, 109, 109, 0.8);
    }
    .content {
        display: flex;
		flex-direction: column;
		align-items: flex-start;
		justify-content: center;
    }
    .groups {
		display: grid;
		grid-template-columns: 1fr 1fr;
		grid-gap: 2rem;
	}
    
    .description {
		position: absolute;
		bottom: 1rem;
		left: 1rem;
		padding: 0.5rem;
		border-radius: 8px;
        font-size: 18px;
        color:#0084f6;
	}
    @media (max-width: 768px) {
		.container {
			width: 80%;
		}
	}
    h2 {
        color: rgba(255, 109, 109, 0.8);
        align-items: center;
        flex-direction: column;
        justify-content: center;
    }
    .project {
		border: 1px solid;
		border-radius: 25px;
		padding: 2rem;
		width: min(60vw, 400px);
		height: min(60vw, 400px);
		display: flex;
		justify-content: center;
		position: relative;
		transition:
			transform 0.2s ease,
			box-shadow 0.2s ease;
	}

	.project:hover {
		transform: scale(1.05);
		box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
	}
    .project-link {
		text-decoration: none;
		color: inherit;
	}

    .project img {
		margin-top: -2rem;
		max-width: 100%;
		height: 75%;
	}
    .tech-list {
		display: flex;
		flex-direction: row;
	}

	.tech {
		margin: 0 0.25rem;
		border: 1px solid white;
		padding: 0.25rem 0.5rem;
		border-radius: 100px;
		font-size: 14px;
	}
    @media (max-width: 1024px) {
		.groups {
			grid-template-columns: 1fr;
		}
	}
</style>