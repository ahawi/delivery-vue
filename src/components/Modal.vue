<template>
  <div
    class="cart-modal__overlay"
    :class="{ open: isOpen }"
    @click.self="closeModal()"
  >
    <div class="cart-modal">
      <div class="cart-modal__header">
        <h2 class="cart-modal__header-title">Корзина</h2>
        <span class="cart-modal__header-close" @click="closeModal()"
          ><img
            src="../assets/images/icons/close-button.svg"
            alt="Закрыть корзину"
            width="25"
            height="25"
            loading="lazy"
        /></span>
      </div>
      <ul class="cart-modal__list">
        <li class="cart-modal__item">
          <p class="cart-modal__item-title">Ролл угорь стандарт</p>
          <span class="cart-modal__item-price">250 ₽</span>
          <div class="cart-modal__item-controls">
            <button class="cart-modal__controls-button">-</button>
            <span class="card-item__controls-count">1</span>
            <button class="cart-modal__controls-button">+</button>
          </div>
        </li>
        <li class="cart-modal__item">
          <p class="cart-modal__item-title">Ролл угорь стандарт</p>
          <span class="cart-modal__item-price">250 ₽</span>
          <div class="cart-modal__item-controls">
            <button class="cart-modal__controls-button">-</button>
            <span class="card-item__controls-count">1</span>
            <button class="cart-modal__controls-button">+</button>
          </div>
        </li>
        <li class="cart-modal__item">
          <p class="cart-modal__item-title">Ролл угорь стандарт</p>
          <span class="cart-modal__item-price">250 ₽</span>
          <div class="cart-modal__item-controls">
            <button class="cart-modal__controls-button">-</button>
            <span class="card-item__controls-count">1</span>
            <button class="cart-modal__controls-button">+</button>
          </div>
        </li>
        <li class="cart-modal__item">
          <p class="cart-modal__item-title">Ролл угорь стандарт</p>
          <span class="cart-modal__item-price">250 ₽</span>
          <div class="cart-modal__item-controls">
            <button class="cart-modal__controls-button">-</button>
            <span class="card-item__controls-count">1</span>
            <button class="cart-modal__controls-button">+</button>
          </div>
        </li>
        <li class="cart-modal__item">
          <p class="cart-modal__item-title">Ролл угорь стандарт</p>
          <span class="cart-modal__item-price">250 ₽</span>
          <div class="cart-modal__item-controls">
            <button class="cart-modal__controls-button">-</button>
            <span class="card-item__controls-count">1</span>
            <button class="cart-modal__controls-button">+</button>
          </div>
        </li>
      </ul>
      <div class="cart-modal__footer">
        <div class="cart-modal__footer-price">1250 ₽</div>
        <div class="cart-modal__footer-controls">
          <button class="cart-modal__footer-button button">
            Оформить заказ
          </button>
          <button class="cart-modal__footer-button button white-bg">
            Отмена
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const { isOpen } = defineProps({ isOpen: Boolean });
const emit = defineEmits(["toggleModal"]);
const closeModal = () => emit("toggleModal");
</script>

<style scoped>
.cart-modal__overlay {
  display: none;
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  align-items: center;
  justify-content: center;
  background: rgba(0, 0, 0, 0.45);
}

.cart-modal__overlay.open {
  display: flex;
}

.cart-modal {
  width: 100%;
  max-width: 780px;
  border-radius: 5px;
  padding: 40px 45px;
  background: var(--color-light);
}

.cart-modal__header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding-bottom: 45px;
}
.cart-modal__header-close {
  cursor: pointer;
}

.cart-modal__list {
  display: flex;
  flex-direction: column;
  row-gap: 15px;
  padding-bottom: 53px;
}

.cart-modal__item {
  display: flex;
  align-items: center;
  flex-direction: row;
  justify-content: space-between;
  border-bottom: 1px solid var(--color-gray);
  padding-right: 15px;
}

.cart-modal__item-title {
  font-size: clamp(14px, 1.6vw, 18px);
}

.cart-modal__item-price {
  font-size: clamp(18px, 1.8vw, 20px);
  font-weight: 700;
  flex: 1;
  text-align: right;
  padding-right: 47px;
  padding-bottom: 3px;
}

.cart-modal__item-controls {
  display: flex;
  flex-direction: row;
  align-items: center;
  column-gap: 14px;
  padding-bottom: 10px;
}

.cart-modal__controls-button {
  font-size: 14px;
  background-color: var(--color-light);
  color: var(--color-blue-light);
  border: 1px solid var(--color-blue-light);
  border-radius: 2px;
  width: 40px;
  height: 32px;
}

.cart-modal__controls-button:hover {
  color: var(--color-dark);
  background-color: var(--color-blue-light);
}

.cart-modal__footer {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.cart-modal__footer-price {
  font-size: clamp(18px, 1.8vw, 20px);
  font-weight: 700;
  color: var(--color-light);
  background-color: #262626;
  border-radius: 5px;
  padding: 15px 20px;
}

.cart-modal__footer-controls {
  display: flex;
  column-gap: 11px;
}

@media (max-width: 625px) {
  .cart-modal {
    padding: 30px 35px;
  }

  .cart-modal__header {
    padding-bottom: 30px;
  }

  .cart-modal__list {
    padding-bottom: 30px;
  }

  .cart-modal__item-price {
    padding-right: 15px;
  }

  .cart-modal__item-controls {
    column-gap: 7px;
  }

  .cart-modal__controls-button {
    font-size: 14px;
    width: 30px;
    aspect-ratio: 1;
  }

  .cart-modal__footer-price {
    padding: 15px 20px;
  }
}

@media (max-width: 450px) {
  .cart-modal {
    padding: 20px 25px;
  }

  .cart-modal__item-title {
    max-width: 130px;
  }

  .cart-modal__footer-controls {
    flex-direction: column;
    row-gap: 10px;
  }
}
</style>
