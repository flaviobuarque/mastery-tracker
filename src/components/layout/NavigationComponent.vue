<template>
	<nav class="container">
		<router-link to="/" class="logo">
			<div class="icon"></div>
			<p><span>Mastery</span></p>
		</router-link>
		<div>
			<router-link
				to="/settings"
				class="icon settings"
				:content="$tc('general.setting', 2)"
				v-tippy="{ placement: 'bottom' }">
				<IconComponent name="cog" />
			</router-link>
		</div>
		<IconComponent name="bars" class="mobile-nav-toggle" @click="$emit('toggleMobileNavigation')" />
	</nav>
</template>
