<template >
  <div>
    <SearchPanel />
    <div class="orders-wrapper">
      <div class="orders-top">
        <h3 class="orders-title">Orders</h3>
        <button class="add-btn">+ Add Order</button>
      </div>
      <OrdersList/>
    </div>
  </div>
</template>
<script>
import SearchPanel from "../../components/Lists/Order/SearchPanel.vue";
import OrdersList from "../../components/Lists/Order/OrdersList.vue";
export default {
  components: {
    SearchPanel,OrdersList
  },
};
</script>
<style lang="scss" scoped>
.orders-wrapper {
}

.orders-top {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 12px 16px;
  border-radius: 6px 6px 0px 0px;
  background-color: #ffffff;
}

.orders-title {
  font-weight: 500;
  font-size: 20px;
  line-height: 24px;
  color: #1d2433;
}

.add-btn {
  padding: 6px 27px;
  width: 170px;
  background-color: $primary;
  border: 1px solid $primary;
  border-radius: 6px;

  font-weight: 700;
  font-size: 16px;
  line-height: 18px;
  text-align: center;
  letter-spacing: 0.01em;
  text-transform: capitalize;
  color: #ffffff;
}
</style>