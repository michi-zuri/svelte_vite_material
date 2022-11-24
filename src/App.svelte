<script>
  import Button, { Label } from '@smui/button';
  import Textfield from '@smui/textfield';
  import Icon from '@smui/textfield/icon';
  import HelperText from '@smui/textfield/helper-text';
  import { Input } from '@smui/textfield';
  let value = '';let a = "hoi";

</script>

<main>
  <div>
    <a href="https://shrine.dev" target="_blank" rel="noreferrer"> 
      <img src="/shrine.svg" class="logo" alt="Shrine Logo" />
    </a>
  </div>
  <h1>hello world</h1>
  <div>
      
    <Textfield variant="filled" bind:value={a} label="Username" required >
      <HelperText slot="helper">has to be unique</HelperText>
    </Textfield>

    <Textfield variant="filled" bind:value={a} label="Password" required type="password" >
      <HelperText slot="helper">has to be secure</HelperText>
    </Textfield>

</div>
  <div class="card">
    <Button on:click={() => alert("you clicked a button!")} variant="raised">
      <Label>Click me!</Label>
    </Button>
  </div>

</main>

<style>
  .logo {
    height: 6em;
    padding: 1.5em;
    text-align:center;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
</style>
