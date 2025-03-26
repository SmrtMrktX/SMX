<script lang="ts">
	import smxLogo from '$lib/img/logo/smxlogo.png';
	let mynavlink = 'text-sm';
</script>

<div class="navbar bg-base-100 shadow-base-200 sticky top-0 z-50 font-extrabold shadow-sm">
	<div class="navbar-start">
		<div class="dropdown z-50 ml-2 p-2">
			<div tabindex="0" role="button" class="btn btn-ghost btn-circle w-14">
				<img class=" rounded-full" src={smxLogo} alt="smx logo" />
			</div>
			<ul class="menu menu-sm dropdown-content bg-base-100 rounded-box mt-3 w-52 p-2 shadow">
				<li><a class={mynavlink} href="/">Home</a></li>
				<li><a class={mynavlink} href="/products">Products</a></li>
				<li><a class={mynavlink} href="/download">Download</a></li>
				<li><a class={mynavlink} href="/about">About</a></li>
			</ul>
		</div>
	</div>
	<div class="fixed top-4 left-1/2 w-full -translate-x-1/2 transform text-center">
		<a href="/" class="btn btn-ghost text-2xl font-extrabold tracking-tight md:text-4xl"
			>SMRT MRKT X
		</a>
		<div class="dropdown dropdown-start text-sm font-extrabold">
			<div tabindex="0" role="button" class="btn rounded-sm font-extrabold text-green-500">V.1</div>
			<ul class="dropdown-content menu bg-base-100 rounded-box z-1 p-2 shadow-sm">
				<li><a href="/">V.1</a></li>
				<li><a href="https://v0.smx.tn">V.0</a></li>
			</ul>
		</div>
	</div>
	<div class="navbar-end">
		<input type="checkbox" value="wireframe" class="toggle theme-controller" />
	</div>
</div>
