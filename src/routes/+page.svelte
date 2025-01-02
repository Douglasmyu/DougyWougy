
<script>
    import Home from './home.svelte';
	import About from './about.svelte';
	import Projects from './projects.svelte';
	import Skills from './skills.svelte';
    import Hobbies from './hobbies.svelte';
    import Connect from './connect.svelte';
	import Toggle from './Toggle.svelte';


</script>
<svelte:head>
    <title>DougyWougy</title>
</svelte:head>
<div id="home">
	<Home />
</div>

<div id="about">
	<About />
</div>

<div id="projects">
	<Projects />
</div>

<div id="skills">
	<Skills />
</div>

<div id="hobbies">
	<Hobbies />
</div>

<div id="connect">
    <Connect />
</div>