<script>
 import SvelteLogo from '../assets/svelte.svg'
import Footer from "../lib/Footer.svelte";
import Header from "../lib/Header.svelte";

</script>

<main class="main-wrapper">
  <Header/>
  <!-- <img src={SvelteLogo} alt="svelte icon"/> -->
  <slot name="body"/>
  <Footer/>
</main>