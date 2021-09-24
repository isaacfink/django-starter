<script>
	import { Router, Link, Route } from "svelte-navigator";
  import Dashboard from './pages/Dashboard.svelte'
  import Employees from './pages/Employees.svelte'
  import Login from './pages/Login.svelte'
  import Nav from './components/Nav.svelte'
</script>

<Router>

	<div>
		<Route path="/">
			<Dashboard />
		</Route>

    	<Route path="/employees">
			<Employees />
		</Route>

		<Route path="/login">
			<Login />
		</Route>
	</div>
</Router>

<style>
  :global(h1){
    outline:none;
  }
  :global(h2){
	outline:none;
  }
</style>