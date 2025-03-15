<script lang="ts">
	import smxLogo from '$lib/img/smxloader.png';
	let mynavlink = 'text-sm';
</script>

<div
	style="	font-family: 'Russo One', sans-serif;
"
	class="navbar bg-base-100 sticky top-0 z-50 shadow-sm"
>
	<div class="navbar-start">
		<div class="dropdown">
			<div tabindex="0" role="button" class="btn btn-ghost btn-circle">
				<img class=" rounded-md border-2 border-white" src={smxLogo} alt="smx logo" />
			</div>
			<ul
				tabindex="0"
				class="menu menu-sm dropdown-content bg-base-100 rounded-box mt-3 w-52 p-2 shadow"
			>
				<li><a class={mynavlink} href="/">Homepage</a></li>
				<li><a class={mynavlink} href="/products">Products</a></li>
				<li><a class={mynavlink} href="/about">About</a></li>
				<li class="text-center font-mono text-xs">version 0.0.4</li>
			</ul>
		</div>
	</div>
	<div class="navbar-center">
		<a href="/" class="btn btn-ghost text-2xl tracking-widest md:text-4xl">SMRT MRKT X </a>
	</div>
	<div class="navbar-end">
		<input type="checkbox" value="dark" class="toggle theme-controller" />
	</div>
</div>
