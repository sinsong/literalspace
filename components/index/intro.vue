<template>
  <div class="intro">
    <span class="name">代码の魔女literal</span>
    <img src="/luna-avatar.png" class="avatar" />
    <p class="describe">肥宅码农</p>
  </div>
</template>

<style scoped>
.intro
{
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items:center;

  height:auto;

  margin: 0px 20px;

  border-radius: 5px;

  background-color: rgba(128, 128, 128, 0.25);
}

.name
{
  font-size: 24px;
  font-weight: normal;
  letter-spacing: 0.15em;

  padding: 5px 25px;

  border-top-left-radius: 5px;
  border-top-right-radius: 5px;

  background-color: rgba(105, 105, 105, 0.36);
}

.avatar
{
  width: 100px;
  height: 100px;

  border-radius:50%;

  margin: 25px;

  transition: all 1s;
}

.avatar:hover
{
  transform: rotate(360deg);
}

.describe
{
  margin-bottom: 20px;
  font-size: 18px;
}
</style>
