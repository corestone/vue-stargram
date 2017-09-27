<template>
	<md-card>
		<md-card-media>
			<img :src="imageUrl">
		</md-card-media>
		<template v-if="fullName">
			<md-card-head>
				<div class="md-title">{{fullName}}</div>
				<div class="md-subhead">@{{username}}</div>
			</md-card-head>
			<md-card-content>
				{{contents}}
			</md-card-content>
		</template>
	</md-card>
</template>

<script>
	export default {
		name: 'Feed',
		props: ['imageUrl', 'fullName', 'username', 'contents']
	}
</script>
<style>

</style>