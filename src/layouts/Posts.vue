<template>
  <div>
    <Post v-for="(post, index) in posts" :key="index" :post="post" />
  </div>
</template>

<script>
import Post from "../components/Post/Post";
export default {
  name: "Posts",
  components: {
    Post,
  },
  data() {
    return {
      posts: [
        {
          accountName: "Justin",
          accountAvatar:
            "https://scontent.fhan2-1.fna.fbcdn.net/v/t1.6435-9/120029977_367000914458532_5592149738590608003_n.jpg?_nc_cat=102&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=xxg3jtmkyh4AX8-WKqt&tn=EMv85PTjACenhtpr&_nc_ht=scontent.fhan2-1.fna&oh=00_AT95ArTA2uJRv0W_VHCePWpmKUqq5l3wj0h7Geb_TtEjyA&oe=625BBAB1",
          liked: false,
          views: 1756081,
          sources: [
            {
              source:
                "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
              type: "video",
            },
          ],
          comments: 8900,
        },
        {
          accountName: "Justin",
          accountAvatar:
            "https://scontent.fhan2-1.fna.fbcdn.net/v/t1.6435-9/120029977_367000914458532_5592149738590608003_n.jpg?_nc_cat=102&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=xxg3jtmkyh4AX8-WKqt&tn=EMv85PTjACenhtpr&_nc_ht=scontent.fhan2-1.fna&oh=00_AT95ArTA2uJRv0W_VHCePWpmKUqq5l3wj0h7Geb_TtEjyA&oe=625BBAB1",
          liked: false,
          views: 1756081,
          sources: [
            {
              source:
                "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
              type: "video",
            },
          ],
          comments: 8900,
        },
        {
          accountName: "Justin",
          accountAvatar:
            "https://scontent.fhan2-1.fna.fbcdn.net/v/t1.6435-9/120029977_367000914458532_5592149738590608003_n.jpg?_nc_cat=102&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=xxg3jtmkyh4AX8-WKqt&tn=EMv85PTjACenhtpr&_nc_ht=scontent.fhan2-1.fna&oh=00_AT95ArTA2uJRv0W_VHCePWpmKUqq5l3wj0h7Geb_TtEjyA&oe=625BBAB1",
          liked: false,
          views: 1756081,
          sources: [
            {
              source:
                "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
              type: "video",
            },
          ],
          comments: 8900,
        },
        {
          accountName: "Justin",
          accountAvatar:
            "https://scontent.fhan2-1.fna.fbcdn.net/v/t1.6435-9/120029977_367000914458532_5592149738590608003_n.jpg?_nc_cat=102&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=xxg3jtmkyh4AX8-WKqt&tn=EMv85PTjACenhtpr&_nc_ht=scontent.fhan2-1.fna&oh=00_AT95ArTA2uJRv0W_VHCePWpmKUqq5l3wj0h7Geb_TtEjyA&oe=625BBAB1",
          liked: false,
          views: 1756081,
          sources: [
            {
              source:
                "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
              type: "video",
            },
          ],
          comments: 8900,
        },
        {
          accountName: "Justin",
          accountAvatar:
            "https://scontent.fhan2-1.fna.fbcdn.net/v/t1.6435-9/120029977_367000914458532_5592149738590608003_n.jpg?_nc_cat=102&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=xxg3jtmkyh4AX8-WKqt&tn=EMv85PTjACenhtpr&_nc_ht=scontent.fhan2-1.fna&oh=00_AT95ArTA2uJRv0W_VHCePWpmKUqq5l3wj0h7Geb_TtEjyA&oe=625BBAB1",
          liked: false,
          views: 1756081,
          sources: [
            {
              source:
                "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
              type: "video",
            },
          ],
          comments: 8900,
        },
        {
          accountName: "Justin",
          accountAvatar:
            "https://scontent.fhan2-1.fna.fbcdn.net/v/t1.6435-9/120029977_367000914458532_5592149738590608003_n.jpg?_nc_cat=102&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=xxg3jtmkyh4AX8-WKqt&tn=EMv85PTjACenhtpr&_nc_ht=scontent.fhan2-1.fna&oh=00_AT95ArTA2uJRv0W_VHCePWpmKUqq5l3wj0h7Geb_TtEjyA&oe=625BBAB1",
          liked: false,
          views: 1756081,
          sources: [
            {
              source:
                "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
              type: "video",
            },
          ],
          comments: 8900,
        },
        {
          accountName: "Justin",
          accountAvatar:
            "https://scontent.fhan2-1.fna.fbcdn.net/v/t1.6435-9/120029977_367000914458532_5592149738590608003_n.jpg?_nc_cat=102&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=xxg3jtmkyh4AX8-WKqt&tn=EMv85PTjACenhtpr&_nc_ht=scontent.fhan2-1.fna&oh=00_AT95ArTA2uJRv0W_VHCePWpmKUqq5l3wj0h7Geb_TtEjyA&oe=625BBAB1",
          liked: false,
          views: 1756081,
          sources: [
            {
              source:
                "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
              type: "video",
            },
          ],
          comments: 8900,
        },
        {
          accountName: "Justin",
          accountAvatar:
            "https://scontent.fhan2-1.fna.fbcdn.net/v/t1.6435-9/120029977_367000914458532_5592149738590608003_n.jpg?_nc_cat=102&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=xxg3jtmkyh4AX8-WKqt&tn=EMv85PTjACenhtpr&_nc_ht=scontent.fhan2-1.fna&oh=00_AT95ArTA2uJRv0W_VHCePWpmKUqq5l3wj0h7Geb_TtEjyA&oe=625BBAB1",
          liked: false,
          views: 1756081,
          sources: [
            {
              source:
                "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
              type: "video",
            },
          ],
          comments: 8900,
        },
        {
          accountName: "Justin",
          accountAvatar:
            "https://scontent.fhan2-1.fna.fbcdn.net/v/t1.6435-9/120029977_367000914458532_5592149738590608003_n.jpg?_nc_cat=102&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=xxg3jtmkyh4AX8-WKqt&tn=EMv85PTjACenhtpr&_nc_ht=scontent.fhan2-1.fna&oh=00_AT95ArTA2uJRv0W_VHCePWpmKUqq5l3wj0h7Geb_TtEjyA&oe=625BBAB1",
          liked: false,
          views: 1756081,
          sources: [
            {
              source:
                "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
              type: "video",
            },
          ],
          comments: 8900,
        },
        {
          accountName: "Justin",
          accountAvatar:
            "https://scontent.fhan2-1.fna.fbcdn.net/v/t1.6435-9/120029977_367000914458532_5592149738590608003_n.jpg?_nc_cat=102&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=xxg3jtmkyh4AX8-WKqt&tn=EMv85PTjACenhtpr&_nc_ht=scontent.fhan2-1.fna&oh=00_AT95ArTA2uJRv0W_VHCePWpmKUqq5l3wj0h7Geb_TtEjyA&oe=625BBAB1",
          liked: false,
          views: 1756081,
          sources: [
            {
              source:
                "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
              type: "video",
            },
          ],
          comments: 8900,
        },
        {
          accountName: "Justin",
          accountAvatar:
            "https://scontent.fhan2-1.fna.fbcdn.net/v/t1.6435-9/120029977_367000914458532_5592149738590608003_n.jpg?_nc_cat=102&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=xxg3jtmkyh4AX8-WKqt&tn=EMv85PTjACenhtpr&_nc_ht=scontent.fhan2-1.fna&oh=00_AT95ArTA2uJRv0W_VHCePWpmKUqq5l3wj0h7Geb_TtEjyA&oe=625BBAB1",
          liked: false,
          views: 1756081,
          sources: [
            {
              source:
                "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
              type: "video",
            },
          ],
          comments: 8900,
        },
        {
          accountName: "Justin",
          accountAvatar:
            "https://scontent.fhan2-1.fna.fbcdn.net/v/t1.6435-9/120029977_367000914458532_5592149738590608003_n.jpg?_nc_cat=102&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=xxg3jtmkyh4AX8-WKqt&tn=EMv85PTjACenhtpr&_nc_ht=scontent.fhan2-1.fna&oh=00_AT95ArTA2uJRv0W_VHCePWpmKUqq5l3wj0h7Geb_TtEjyA&oe=625BBAB1",
          liked: false,
          views: 1756081,
          sources: [
            {
              source:
                "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
              type: "video",
            },
          ],
          comments: 8900,
        },
        {
          accountName: "Justin",
          accountAvatar:
            "https://scontent.fhan2-1.fna.fbcdn.net/v/t1.6435-9/120029977_367000914458532_5592149738590608003_n.jpg?_nc_cat=102&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=xxg3jtmkyh4AX8-WKqt&tn=EMv85PTjACenhtpr&_nc_ht=scontent.fhan2-1.fna&oh=00_AT95ArTA2uJRv0W_VHCePWpmKUqq5l3wj0h7Geb_TtEjyA&oe=625BBAB1",
          liked: false,
          views: 1756081,
          sources: [
            {
              source:
                "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
              type: "video",
            },
          ],
          comments: 8900,
        },
        {
          accountName: "Justin",
          accountAvatar:
            "https://scontent.fhan2-1.fna.fbcdn.net/v/t1.6435-9/120029977_367000914458532_5592149738590608003_n.jpg?_nc_cat=102&ccb=1-5&_nc_sid=09cbfe&_nc_ohc=xxg3jtmkyh4AX8-WKqt&tn=EMv85PTjACenhtpr&_nc_ht=scontent.fhan2-1.fna&oh=00_AT95ArTA2uJRv0W_VHCePWpmKUqq5l3wj0h7Geb_TtEjyA&oe=625BBAB1",
          liked: false,
          views: 1756081,
          sources: [
            {
              source:
                "https://o.rada.vn/data/image/2020/12/14/thuyet-minh-ve-loai-cho.jpg",
              type: "video",
            },
          ],
          comments: 8900,
        },
      ],
    };
  },
};
</script>

<style>
</style>