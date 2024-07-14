<template>
 <footer class="footer">
			<div class="container">
				<div class="footer-box">
					<router-link to="/" class="footer-logo logo">
						<img src="../assets/img/icon/logo.svg" alt="logo" />
					</router-link>
					<div class="footer-nav">
						<ul>
							<li> Ресторанам</li>
							<li>Курьерам</li>
							<li>Пресс-центр></li>
							<li>Контакты</li>
						</ul>
					</div>
					<div class="footer-social">
						<img src="../assets/img/social/instagram.svg" alt="instagram" />
						<img src="../assets/img/social/fb.svg" alt="facebook" />
						<img src="../assets/img/social/vk.svg" alt="vk" />
					</div>
				</div>
				<!-- /.footer-box -->
			</div>
		</footer> 
</template>

<script>
export default {

}
</script>

<style scoped>
.footer {
    min-height: 156px;
    display: flex;
    align-items: center;
    padding: 60px 0;
}

.footer-box {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 36px;
    flex-wrap: wrap;
}

.footer-nav {
    flex-grow: 1;
}

.footer-nav ul {
    display: flex;
    align-items: center;
    list-style: none;
    margin: 0;
    padding: 0;
    gap: 15px;
    flex-wrap: wrap;
}

.footer-nav ul li {
    color: #595959;
    font-size: 18px;
    font-weight: 400;
    text-decoration: none;
}
.footer-nav ul li a{
    text-decoration: none; 
}
.footer-social {
    display: flex;
    align-items: center;
    justify-content: flex-end;
    gap: 20px;
}
</style>