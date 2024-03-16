<script>
  import {Link} from 'svelte-routing'
  import svelteLogo from '../assets/svelte.svg'
</script>


<header>
  <img src={svelteLogo} alt="header-logo"/>
  <nav>
    <ul>
      <li>
        <Link to="/">Home</Link>
      </li>
      <li>
        <Link to="/profile">
          Profile
        </Link>
      </li>
      <li>
        <Link to="/games">
          Games
        </Link>
      </li>
    </ul>
  </nav>
</header>


<style>

  header{
    display: flex;
    justify-content: space-between;
    background: wheat;
    padding: 8px;
    align-items: center;
  }
  
  ul{
    display: flex;
    list-style: none;
    padding-inline-start: 0;
    gap: 16px;
    text-decoration: none;
  }

  :global(nav ul li a){
    text-decoration: none;
  }
</style>
