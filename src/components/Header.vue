<template>
    <header class="header">
			<div class="container">
				<div class="header-box">
					<router-link to="/" class="header-logo logo">
						<img src="../assets/img/icon/logo.svg" alt="Logo" />
					</router-link>
					<div class="header-controls">
						<button class="btn btn-primary">
							<img class="btn-auth-svg" src="../assets/img/icon/user.svg" alt="user"/>
							<span class="button-text">Войти</span>
						</button>
						<button class="btn btn-outline" @click="openModal()">
							<img class="btn-cart-svg" src="../assets/img/icon/shopping-cart.svg" alt="cart"/>
							<span class="button-text">Корзина</span>
						</button>

					</div>
				</div>
			</div>
		</header>
</template>

<script setup>
const emit=defineEmits(['toggleModal'])
const openModal=()=>{emit('toggleModal')}
</script>

<style  scoped>
.header {
    display: flex;
    align-items: center;
    min-height: 124px;
}

.header-box {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
</style>