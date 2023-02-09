<script>
	export default {
		data() {
      return {
        visible: true,
	}
  },
  methods: {
	hide: function() {
		this.visible = false;
	},
  mide: function() {
		this.visible = true;
	}
}
  
	}
</script>
<template>
  <button @click="hide">hide</button>
  <button @click="visible">visible</button>
	<p v-if="visible">text</p>
</template>

<style>

</style>
