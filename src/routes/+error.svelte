<script lang="ts">
import { page } from '$app/state';
const message = page.error?.message ?? 'Unknown error';
</script>

<h1>ERROR PAGE!</h1>

{page.status}: {message}