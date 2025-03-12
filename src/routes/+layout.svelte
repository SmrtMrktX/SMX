<script lang="ts">
	import smxLogo from '$lib/img/smxloader.png';
	import '../app.css';
	let { children } = $props();
</script>

<div class="navbar bg-base-100 sticky top-0 shadow-sm">
	<div class="navbar-start">
		<div class="dropdown">
			<div tabindex="0" role="button" class="btn btn-ghost btn-circle">
				<img class=" rounded-md border-2 border-white" src={smxLogo} alt="smx logo" />
			</div>
			<ul
				tabindex="0"
				class="menu menu-sm dropdown-content bg-base-100 rounded-box z-1 mt-3 w-52 p-2 shadow"
			>
				<li><a>Homepage</a></li>
				<li><a>Portfolio</a></li>
				<li><a>About</a></li>
				<li class="text-center font-mono text-xs">Version 0.0.4</li>
			</ul>
		</div>
	</div>
	<div class="navbar-center">
		<a class="btn btn-ghost text-2xl font-extrabold">SMRT MRKT X </a>
	</div>
	<div class="navbar-end">
		<input type="checkbox" value="black" class="toggle theme-controller" />
	</div>
</div>

{@render children()}
