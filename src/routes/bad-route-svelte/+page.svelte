<script lang="ts">
  import { error } from "@sveltejs/kit";

  throw error(500, 'This is an error in the route setup');
</script>

<h1>Bad route</h1>