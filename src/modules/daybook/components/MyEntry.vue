<template>
	<div class="entry-container mb-3 pointer p-2" @click="$router.push({ name:'entry', params:{id:10} } )">
		<div class="entry-title d-flex">
			<span class="text-success fs-5 fw-bold">2</span>
			<span class="mx-1 fs-5">Mayo</span>
			<span class="mx-2 fw-light">2022, lunes</span>
		</div>
		<div class="entry-description">
			Lorem ipsum, dolor sit amet consectetur adipisicing elit. Enim assumenda odit animi distinctio voluptatibus dolores sed ipsam et ullam suscipit veritatis voluptate, numquam similique soluta excepturi molestiae dicta deserunt magnam?
		</div>
	</div>
</template>

<script>
export default {
	name:'MyEntry'

}
</script>

<style lang='scss' scoped>

.entry-container{
	border-bottom: 1px solid #2c3e50;
	transition: 0.2s all ease-in;

	&:hover{
		background-color: lighten($color: grey, $amount: 45);
		transition: .2s all ease-in;
	}

	.entry-description{
		font-size: 12px;
	}
}

</style>