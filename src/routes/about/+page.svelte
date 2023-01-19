  
<script>

import List, { Group, Item, Subheader} from '@smui/list';
import FilterGroup from '../../FilterGroup.svelte';
import PaperCard from '../../PaperCard.svelte';

$: innerHeight = 0;
$: innerWidth = 0;

</script>

<svelte:window bind:innerHeight bind:innerWidth />

<div class="container">
    <div style="height: {innerHeight - 22}px; width: 20%;" class="demo-cell">
        <Group>
            <Subheader>Catagory 1</Subheader>
            <List class="demo-list">
                <FilterGroup></FilterGroup>
            </List>
          </Group>
          <Group>
            <Subheader>Catagory 2</Subheader>
            <List class="demo-list">
                <FilterGroup></FilterGroup>
            </List>
          </Group>
    </div>

    <div style="height: {innerHeight - 22}px; width: 55%;" class="demo-cell">
        
    </div>

    <div style="height: {innerHeight - 22}px; width: 25%;" class="demo-cell">
        <PaperCard></PaperCard>
        <PaperCard></PaperCard>
    </div>
</div>



<style>
    .container {
    display: flex; /* or inline-flex */
    align-items: center;
    }

    .demo-cell {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin: 10px;
      border: 1px;
      border-style: solid;
      border-color: var(--mdc-theme-secondary, #333);
      color: var(--mdc-theme-secondary, rgb(15, 9, 9));
    }

    * :global(.demo-list) {
    max-width: 600px;
    border-left: 1px solid
      var(--mdc-theme-text-hint-on-background, rgba(0, 0, 0, 0.1));
  }
</style>
  