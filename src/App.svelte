<script>
		import Home from "./pages/Home/Home.svelte";
		import Recepies from "./pages/Recepies/Recepies.svelte";
		import Items from "./pages/Items/Items.svelte";
    import { Router, Link, Route } from "svelte-routing";
</script>

<Router>
	<nav>
		<div class="nav-wrapper">
			<ul>
				<li><Link to="/">Home</Link></li>
			</ul>
			<ul id="nav-mobile" class="right hide-on-med-and-down">
				<li><Link to="recepies">Recepies</Link></li>
				<li><Link to="items">Items</Link></li>
			</ul>
		</div>
	</nav>
	<div>
		<Route path="/" component={Home} />
		<Route path="recepies" component={Recepies} />
		<Route path="items" component={Items} />
	</div>
</Router>