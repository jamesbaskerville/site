<template>
  <q-page class="flex flex-center">
    <q-btn
      label="Do something"
      @click="$q.notify('something')"
    />
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
};
</script>
