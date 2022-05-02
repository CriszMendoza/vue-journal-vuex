<template>
	<MyNavbar/>
	<div class="d-flex">
		<div class="col-4">
			<EntryList/>
		</div>
		<div class="col-8">
			<router-view/>
		</div>
	</div>
</template>

<script>

import { defineAsyncComponent } from 'vue'

export default {
	components:{
		MyNavbar: defineAsyncComponent(()=> import('../components/MyNavbar.vue')),
		EntryList: defineAsyncComponent(()=> import('../components/EntryList.vue'))
	}

}
</script>

<style>

</style>