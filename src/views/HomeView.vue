<template>
  <section class="container">
    <div class="hero">
      <div class="hero__inner">
        <h1 class="hero__title">Онлайн-сервис доставки еды на дом</h1>
        <p class="hero__description">
          Блюда из любимого ресторана привезет курьер в перчатках, маске и с
          антисептиком
        </p>
      </div>
    </div>
  </section>

  <section class="container">
    <div class="rests">
      <div class="rests__header">
        <h2 class="rests__header-title">Рестораны</h2>
        <div class="rests__header-search">
          <svg
            width="16"
            height="16"
            viewBox="0 0 16 16"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M14.9891 14.0205L10.424 9.45547C11.1324 8.53965 11.5156 7.41992 11.5156 6.24219C11.5156 4.83242 10.9654 3.51055 9.97051 2.51387C8.97559 1.51719 7.6502 0.96875 6.24219 0.96875C4.83418 0.96875 3.50879 1.51895 2.51387 2.51387C1.51719 3.50879 0.96875 4.83242 0.96875 6.24219C0.96875 7.6502 1.51895 8.97559 2.51387 9.97051C3.50879 10.9672 4.83242 11.5156 6.24219 11.5156C7.41992 11.5156 8.53789 11.1324 9.45371 10.4258L14.0188 14.9891C14.0321 15.0025 14.048 15.0131 14.0655 15.0203C14.083 15.0276 14.1018 15.0313 14.1207 15.0313C14.1396 15.0313 14.1584 15.0276 14.1759 15.0203C14.1934 15.0131 14.2093 15.0025 14.2227 14.9891L14.9891 14.2244C15.0025 14.211 15.0131 14.1951 15.0203 14.1776C15.0276 14.1601 15.0313 14.1414 15.0313 14.1225C15.0313 14.1035 15.0276 14.0848 15.0203 14.0673C15.0131 14.0498 15.0025 14.0339 14.9891 14.0205V14.0205ZM9.02656 9.02656C8.28125 9.77012 7.29336 10.1797 6.24219 10.1797C5.19102 10.1797 4.20313 9.77012 3.45781 9.02656C2.71426 8.28125 2.30469 7.29336 2.30469 6.24219C2.30469 5.19102 2.71426 4.20137 3.45781 3.45781C4.20313 2.71426 5.19102 2.30469 6.24219 2.30469C7.29336 2.30469 8.28301 2.7125 9.02656 3.45781C9.77012 4.20313 10.1797 5.19102 10.1797 6.24219C10.1797 7.29336 9.77012 8.28301 9.02656 9.02656Z"
              fill="#8C8C8C"
            />
          </svg>
          <input
            type="search"
            class="rests__header-input white-bg"
            id="search-input"
            name="search"
            placeholder="Поиск блюд и ресторанов"
          />
        </div>
      </div>
      <ul class="rests__list grid">
        <li class="rests__item" v-for="rest in store.rests" :key="rest.id">
          <router-link :to="`/rest?id=${rest.id}`" class="rests__link">
            <img
              class="rests__item-image"
              :src="getUrl(rest.image)"
              alt="Пицца плюс"
              width="384"
              height="250"
              loading="lazy"
            />
            <div class="rests__item-body">
              <div class="rests__item-header">
                <h3 class="rests__item-title">{{ rest.title }}</h3>
                <span class="rests__item-time">{{ rest.time }} мин</span>
              </div>

              <div class="rests__item-description">
                <span class="rests__item-description-rating">{{
                  rest.rating
                }}</span>
                <span class="rests__item-description-price"
                  >От {{ rest.price }} ₽</span
                >
                <span class="rests__item-description-category">{{
                  rest.type
                }}</span>
              </div>
            </div>
          </router-link>
        </li>
      </ul>
    </div>
  </section>
</template>

<script setup>
import { store } from "../store/index";
const getUrl = (name) => {
  return new URL(`../assets/images/rests/${name}`, import.meta.url);
};
</script>
