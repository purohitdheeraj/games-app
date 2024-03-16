<script lang="ts">
  import {Router, Route} from 'svelte-routing'
	import Layout from './layout/Layout.svelte';
	import Profile from './lib/Profile.svelte';
	import Games from './lib/Games.svelte';

</script>

<Router>
<main>
    <Layout>
      <div slot="body" class="main-content">
        <Route path="/">Home</Route>
        <Route path="/profile" component={Profile}/>
        <Route path="/games" component={Games}/>
      </div>
    </Layout>
</main>

</Router>

<style>
  .main-content{
    height: 86vh;
    border: 1px solid;
  }
</style>