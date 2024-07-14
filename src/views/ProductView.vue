<template>
	 <section class="products">
                <div class="container">
                    <div class="products-wrapper" id="goods-container">
                        <div class="products-card"  v-for="good in goodsArray" :key="good.id">
                            <div class="products-card__image"  >
                                <img :src="getUrl(good.image)"  alt="good-1" />
                            </div>
                            <div class="products-card__description">
                                <div class="products-card__description-row">
                                    <h5 class="products-card__description--name">
                                        {{ good.name }} 
                                    </h5>
                                </div>
                                <div class="products-card__description-row">
                                    <p class="products-card__description--text">
                                        {{ good.compound }} 
                                    </p>
                                </div>
                                <div class="products-card__description-row">
                                    <div class="products-card__description-controls">
                                        <button class="btn btn-primary">
                                            <span class="button-text">В корзину</span>
                                            <img src="../assets/img/icon/shopping-cart-white.svg" alt="shopping-cart" />
                                        </button>
                                        <span class="products-card__description-controls--price">
                                            {{ good.price }} ₽
                                        </span>
                                    </div>
                                </div>
                            </div>
                        </div>
                       
                       
                    </div>
                </div>
                <!-- /.container -->
            </section>
</template>
<script setup>
import {goodsArray} from "../constants/goods"
const getUrl=(name) =>{
	return new URL(`../assets/img/goods/${name}`, import.meta.url)
}
</script>
