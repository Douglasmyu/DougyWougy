<script>
    let activeTab = 'languages';
    const languages = ['C++', 'C#', 'Python', 'JavaScript', "swift", 'HTML/CSS', 'SQL'];
    const tools = ['Unity','Git/Github', 'Xcode'];
</script>
<section class = "container">
    <div class = "content">
        <h1 class = "title">Skills</h1>
        <div class = "tabs">
            <button class="tab-button"
            on:click={() => (activeTab = 'languages')}
            class:active={activeTab === 'languages'}>
                Languages
            </button>
            <button class="tab-button"
            on:click={() => (activeTab = 'tools')}
            class:active={activeTab === 'tools'}>
                Tools
            </button>
        </div>
        <div class="tab-content">
			{#if activeTab === 'languages'}
				{#each languages as lang}
					<div class="skill-item">{lang}</div>
				{/each}
			{:else if activeTab === 'tools'}
				{#each tools as tool}
					<div class="skill-item">{tool}</div>
				{/each}
			{/if}
		</div>
    </div>
</section>

<style>
    .container{
        display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		width: 100%;
		height: 100vh;
		margin: 0 auto;
        background-color: #f2eee2;
    }
    .content {
        margin-top: 10%;
		display: flex;
		flex-direction: column;
		/* align-items: center; */
		width: 60%;
        color: #0084f6;
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
    .tabs {
		display: flex;
		justify-content: flex-start;
		gap: 1rem;
		margin-bottom: 1rem;
		width: 100%;
	}
	.tab-button {
		padding: 0.5rem 1rem;
		border: none;
		background-color: transparent;
        color:rgba(255, 109, 109, 0.8);
		cursor: pointer;
		border-radius: 1000px;
		transition: background-color 0.3s ease;
	}

	.tab-button.active {
		background-color: none;
		border: 1px solid white;
		color: white;
	}

	.tab-content {
		display: flex;
		/* justify-content: center; */
		flex-wrap: wrap;
		gap: 0.5rem;
	}

	.skill-item {
		width: calc(50% - 3rem);
		padding: 0.5rem 1rem;
		background-color: #353535;
		margin: 0;
	}
    @media (max-width: 768px) {
		.content {
			width: 80%;
		}

		.skill-item {
			width: 100%;
		}
	}
</style>