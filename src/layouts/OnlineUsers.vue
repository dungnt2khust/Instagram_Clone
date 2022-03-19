<template>
  <div class="online-user position-relative p-v-16">
    <div
      @click="scrollOnlineUsers(true)"
      class="users__next cur-p mi-next position-absolute"
    ></div>
    <div
      @click="scrollOnlineUsers(false)"
      class="users__previous cur-p mi-previous position-absolute"
    ></div>
    <div class="users d-flex m-h-8">
      <div
        class="user d-flex flex-column align-items-center m-h-4"
        v-for="(user, index) in onlineUsers"
        :title="user.accountName"
        :key="index"
      >
        <div class="user__avatar-wrapper mi-66">
          <div
            class="user__avatar mi-62"
            :style="{ 'background-image': `url('${user.accountAvatar}')` }"
          ></div>
        </div>
        <div class="user__name m-t-4">{{ user.accountName }}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "OnlineUsers",
  data() {
    return {
      onlineUsers: [
        {
          accountId: 2314,
          accountName: "_dungnguyentien_",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },
        {
          accountId: 2314,
          accountName: "_npt__",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },
        {
          accountId: 2314,
          accountName: "asdfasf",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },
        {
          accountId: 2314,
          accountName: "asdfasf",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },
        {
          accountId: 2314,
          accountName: "asdfasf",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },
        {
          accountId: 2314,
          accountName: "asdfasf",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },
        {
          accountId: 2314,
          accountName: "asdfasf",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },
        {
          accountId: 2314,
          accountName: "asdfasf",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },

        {
          accountId: 2314,
          accountName: "asdfasf",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },
        {
          accountId: 2314,
          accountName: "asdfasf",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },
        {
          accountId: 2314,
          accountName: "asdfasf",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },
        {
          accountId: 2314,
          accountName: "asdfasf",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },
        {
          accountId: 2314,
          accountName: "asdfasf",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },
        {
          accountId: 2314,
          accountName: "asdfasf",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },
        {
          accountId: 2314,
          accountName: "asdfasf",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },
        {
          accountId: 2314,
          accountName: "asdfasf",
          accountAvatar:
            "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
        },
      ],
    };
  },
  methods: {
    scrollOnlineUsers(isNext) {
      console.log(isNext);
      console.log(document);
    },
  },
};
</script>

<style lang="scss">
.online-user {
  &::-webkit-scrollbar {
    display: none;
  }
  width: 600px;
  overflow: scroll;
  border: 1px solid #DBDBDB;
  .users__next {
    right: 0;
    top: 50%;
    transform: translateY(-50%);
  }
  .users__previous {
    left: 0;
    top: 50%;
    transform: translateY(-50%);
  }
  .user {
    user-select: none;
    cursor: pointer;
    min-width: 74px;
    .user__avatar-wrapper {
      border-radius: 50%;
      border: 2px solid transparent;
      background-image: linear-gradient(white, white),
        radial-gradient(circle at top left, rgb(252, 45, 200), #ff7220);
      background-origin: border-box;
      background-clip: content-box, border-box;
      .user__avatar {
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        border-radius: 50%;
        border: 2px solid #fff;
      }
    }
    .user__name {
      letter-spacing: 0.01em;
      max-width: 74px;
      overflow: hidden;
      text-align: center;
      text-overflow: ellipsis;
      white-space: nowrap;
      color: #262626;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
        Helvetica, Arial, sans-serif;
      font-size: 12px;
    }
  }
}
</style>