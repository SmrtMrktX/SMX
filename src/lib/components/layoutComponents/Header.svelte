<script lang="ts">
	import smxLogo from '$lib/img/logos/faviconB.png';
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
				<img class=" rounded-md" src={smxLogo} alt="smx logo" />
			</div>
			<ul
				tabindex="0"
				class="menu menu-sm dropdown-content bg-base-100 rounded-box mt-3 w-52 p-2 shadow"
			>
				<li><a class={mynavlink} href="/">Homepage</a></li>
				<li><a class={mynavlink} href="/products">Products</a></li>
				<li><a class={mynavlink} href="/about">About</a></li>
			</ul>
		</div>
	</div>
	<div class="navbar-center">
		<a href="/" class="btn btn-ghost text-2xl tracking-widest md:text-4xl">SMRT MRKT X </a>
	</div>
	<div class="navbar-end">
		<div class="dropdown dropdown-start mr-4 text-sm">
			<div tabindex="0" role="button" class="btn m-1">V.1 beta</div>
			<ul tabindex="0" class="dropdown-content menu bg-base-100 rounded-box z-1 ml-1 p-2 shadow-sm">
				<li><a href="/">V.1</a></li>
				<li><a href="https://v0.smx.tn" target="_blank">V.0</a></li>
			</ul>
		</div>
		<input type="checkbox" value="wireframe" class="toggle theme-controller" />
	</div>
</div>
