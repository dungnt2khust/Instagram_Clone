<template>
  <div class="controls d-flex">
    <Icon_Home class="m-l-22 cur-p" title="Home" />
    <Icon_Messenger class="m-l-22 cur-p" title="Messenger" />
    <Icon_New class="m-l-22 cur-p" title="New post" />
    <Icon_FindPeople class="m-l-22 cur-p" title="Find people" />
    <Icon_Heart class="m-l-22 cur-p" title="Activity" />
    <div class="mi-24 m-l-22 cur-p" title="Accounts">
      <img
        src="https://scontent.fhan2-1.fna.fbcdn.net/v/t1.6435-9/120029977_367000914458532_5592149738590608003_n.jpg?_nc_cat=102&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=xxg3jtmkyh4AX8-WKqt&tn=EMv85PTjACenhtpr&_nc_ht=scontent.fhan2-1.fna&oh=00_AT95ArTA2uJRv0W_VHCePWpmKUqq5l3wj0h7Geb_TtEjyA&oe=625BBAB1"
        alt="Avatar"
        class="controls__avatar"
      />
    </div>
  </div>
</template>

<script>
import Icon_Home from "../Icons/Icon_Home";
import Icon_Messenger from "../Icons/Icon_Messenger";
import Icon_New from "../Icons/Icon_New";
import Icon_FindPeople from "../Icons/Icon_FindPeople";
import Icon_Heart from "../Icons/Icon_Heart";
export default {
  name: "Controls",
  components: {
    Icon_FindPeople,
    Icon_Heart,
    Icon_Messenger,
    Icon_New,
    Icon_Home,
  },
};
</script>

<style lang="scss">
.controls {
  .controls__avatar {
    width: 24px;
    height: 24px;
    border-radius: 50%;
  }
}
</style>