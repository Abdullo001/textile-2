<template >
  <div class="header-wrapper">
    <div class="header-container">
     <h2 class="header-title">Lists</h2>
 
     <input type="search" class="search-input" placeholder="Search" />
 
     <div class="profile">
       <img src="~assets/images/Notification.svg" alt="" class="notification" />
 
       <select id="" class="lang">
         <option value="en">EN</option>
         <option value="ru">РУ</option>
         <option value="uz">UZ</option>
       </select>
 
       <div class="profile-info">
         <div class="profile-info-box">
           <span class="profile-name">Asadbek Bektayev</span>
           <span class="profile-status">Admin</span>
         </div>
         <img src="~assets/images/profilePicture.png" alt="" />
       </div>
     </div>
    </div>
 
    <div class="header-link-box">
     <span>Lists / Orders</span>
     
    </div>
   </div>
</template>
<script>
export default {
  
}
</script>
<style scoped lang="scss" >
.header-wrapper {
  width: 100%;

  background-color: #ffffff;
}

.header-container{
  display: flex;
  align-items: center;
  padding: 15px 24px 6px;
  
  border-bottom: 1px solid #dfdfdf;
}

.header-title {
  margin-right: 341px;
  font-weight: 700;
  font-size: 20px;
  line-height: 24px;
  color: #777c85;
}

.search-input {
  width: 320px;
  margin-right: 37px;
  padding: 6px 16px;
  padding-left:36px ;
  border: 1px solid #d2d3d6;
  border-radius: 8px;
  background: transparent url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' class='bi bi-search' viewBox='0 0 16 16'%3E%3Cpath d='M11.742 10.344a6.5 6.5 0 1 0-1.397 1.398h-.001c.03.04.062.078.098.115l3.85 3.85a1 1 0 0 0 1.415-1.414l-3.85-3.85a1.007 1.007 0 0 0-.115-.1zM12 6.5a5.5 5.5 0 1 1-11 0 5.5 5.5 0 0 1 11 0z'%3E%3C/path%3E%3C/svg%3E") no-repeat 13px center;
}

.profile {
  display: flex;
  align-items: center;
}

.notification {
  display: inline-block;
  margin-right: 35px;
}

.lang {
  margin-right: 48px;
  padding: 8px 8px;
  background: #f4f5fa;
  border-radius: 5px;
}

.profile-info {
  display: flex;
  align-items: center;
}

.profile-info-box {
  display: flex;
  flex-direction: column;
  align-items: end;
  margin-right: 10px;
}

.profile-name {
  font-weight: 700;
  font-size: 14px;
  line-height: 20px;
  color: #1d2433;
}

.header-link-box{
  padding: 6px 24px 6px;
  
}
</style>