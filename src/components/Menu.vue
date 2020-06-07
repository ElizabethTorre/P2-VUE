<template>
	<div>
		<b-button variant="primary">{{tema.area}}</b-button>
	</div>
</template>
<script>
	//import {db} from '../main';
	export default {
		name: 'Menu',
		props: {
			tema: {
				type: Object,
				required: true
			}
		}
	}
</script>
