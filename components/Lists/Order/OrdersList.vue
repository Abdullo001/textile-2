<template >
  <div>
    <div class="list-top">
      <div class="checkbox-wrapper">
        <input type="checkbox" name="" id="" />
      </div>
      <span class="order-name"
        >Order number <img src="~assets/images/sort.svg" alt=""
      /></span>
      <span class="model"
        >Model <img src="~assets/images/sort.svg" alt=""
      /></span>
      <span class="client-name"
        >Client Name <img src="~assets/images/sort.svg" alt=""
      /></span>
      <span class="created-by"
        >Created by <img src="~assets/images/sort.svg" alt=""
      /></span>
      <span class="created-at"
        >Created at <img src="~assets/images/sort.svg" alt=""
      /></span>
      <span class="status"
        >Status <img src="~assets/images/sort.svg" alt=""
      /></span>
      <span class="deadline"
        >Deadline <img src="~assets/images/sort.svg" alt=""
      /></span>
      <span class="toolbar"
        ><img src="~assets/images/options.svg" alt=""
      /></span>
    </div>
    <ul class="orders-list">
      <li class="orders-item">
        <div class="checkbox-wrapper">
          <input type="checkbox" name="" id="" />
        </div>
        <span class="order-name">12345 </span>
        <div class="model">
          <img
            src="~assets/images/order-avatar.png"
            class="order-avatar"
            width="38"
            height="38"
            alt="order-avatar"
          />
          <div class="order-info">
            <span class="order-type"> T-shirt </span>

            <span class="order-serial-number">
              3803-07-0281
              <img src="~/assets/images/u_copy-alt.svg" alt="" />
            </span>
          </div>
        </div>
        <span class="client-name">Asadbek </span>
        <span class="created-by">Hamidullayev A </span>
        <div class="created-at">
          <span class="order-created-date"> 12.10.2022 </span>
          <span class="order-created-time"> 12:25:08 </span>
        </div>
        <div class="status">
          <select class="status-select pending">
            <option value="">In process</option>
            <option value="">Pending</option>
            <option value="">Cancelled</option>
            <option value="">Finished</option>
          </select>
        </div>
        <span class="deadline">
          <span class="order-deadline-date"> 12.10.2022 </span>
          <span class="order-deadline-time"> 12:25:08 </span>
        </span>
        <span class="toolbar"
          ><img src="~assets/images/options.svg" alt=""
        /></span>
      </li>
    </ul>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
.list-top {
  display: flex;
  align-items: center;
  padding: 10px 0;
  background-color: #f4f5fa;
  border-bottom: 1px solid #e9eaeb;

  font-weight: 500;
  font-size: 14px;
  line-height: 20px;
  color: #6b7280;
}
.checkbox-wrapper,
.model,
.order-name,
.client-name,
.created-by,
.created-at,
.status,
.deadline,
.toolbar {
  display: flex;
  align-items: center;
  padding-left: 8px;
}

.model,
.order-name,
.client-name,
.created-by,
.created-at,
.status,
.deadline {
  img {
    padding-left: 2px;
  }
}

.checkbox-wrapper {
  padding-right: 8px;
}

.order-name {
  width: 150px;
}

.model {
  width: 271px;
}

.client-name {
  width: 140px;
}

.created-by {
  width: 166px;
}

.created-at {
  width: 120px;
}

.status {
  width: 130px;
}

.deadline {
  width: 125px;
}

.toolbar {
  padding-right: 8px;
}

.orders-list {
  list-style-type: none;

  background-color: #ffffff;
}

.orders-item {
  display: flex;
  align-items: center;

  padding: 8px 0;

  .created-at,
  .deadline {
    display: flex;
    flex-direction: column;
    align-items: start;
  }
}

.order-avatar {
  margin: 0;
  padding: 0;
  margin-right: 8px;
}

.order-info {
  display: flex;
  flex-direction: column;

  .order-serial-number {
    display: flex;
    align-items: center;

    font-weight: 400;
    font-size: 14px;
    line-height: 20px;
    color: #777c85;
  }
}

.status-select {
  display: block;
  padding: 4px 10px;
  width: 100px;

  border-radius: 10px;

  font-weight: 500;
  font-size: 12px;
  line-height: 12px;
  text-align: center;
}

.finished {
  background-color: #d1fae5;
  color: $success;
}

.cancelled {
  background-color: #fee2e2;
  color: $error;
}

.pending {
  background-color: #fef3c7;
  color: $warning;
}

.process {
  background-color: #dbeafe;
  color: $secondary;
}

.order-created-time,
.order-deadline-time {
  display: inline-block;
  font-weight: 400;
  font-size: 14px;
  line-height: 20px;
  color: #777c85;
}
</style>