<script>
  import TopAppBar, {Row, Section, Title} from "@smui/top-app-bar";
  import { Router, Link, Route } from "svelte-routing";
  import About from "./About.svelte";
  import Clients from "./Clients.svelte";
  import NavLink from "./NavLink.svelte";
  import Button, {Label} from '@smui/button';
  export let username;
</script>

<style>
  @media screen and (max-width: 800px) {
    .user {
      display: none;
    }
  }
</style>

<TopAppBar variant="static" color="primary">
  <Row>
    <Section>
      <Title>WireGuard VPN</Title>
    </Section>
    <Section align="end" toolbar>
      <Button href="/oauth2/sign_out"><Label>Sign Out</Label></Button>
    </Section>
  </Row>
</TopAppBar>
