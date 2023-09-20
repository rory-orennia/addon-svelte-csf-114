<script context="module" lang="ts">
  
  import Test from './Test.svelte'
  
  export const meta = {
    title: 'Inputs/Test',
    component: Test,
  }
</script>

<script>
  import { Story, Template } from '@storybook/addon-svelte-csf';
</script>

<Template let:args>
  <Test {...args} />
</Template>

<Story name="Story1" args={{ text: 'Story1' }} />
<Story name="Story2" args={{ text: 'Story2' }} />
<Story name="Story3" args={{ text: 'Story3' }} />