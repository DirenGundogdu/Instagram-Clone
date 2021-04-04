<template>
  <div class="post">

      <!-- header -->
          <header class="header section">
            <div class="header-author">
              <Avatar :size="30"/>
            <div class="header-author-info">
              <div><CustomText tag="b" >direngundogdu</CustomText></div>
              <div><CustomText  size="xsmall">Milky Way Galaxy, Earth</CustomText></div>



            </div>
            </div>
            <div class="header-more">
              <button type="button">
                <IconMore/>
              </button>
            </div>
          </header>
      <!-- media -->
      <div class="post-media">
        <img src="https://images.unsplash.com/photo-1444703686981-a3abbc4d4fe3?ixid=MXwxMjA3fDB8MHxzZWFyY2h8MXx8cGljdHVyZXxlbnwwfHwwfA%3D%3D&ixlib=rb-1.2.1&w=1000&q=80" alt="">
      </div>

      <!-- action -->
        <div class="action-buttons section">

          <button type="button">
            <IconLike/>
          </button>
          <button type="button">
            <IconComment/>
          </button>
          <button type="button">
            <IconDirect/>
          </button>
          <button class="action-save" type="button">
            <IconSave/>
          </button>
        </div>

      <!-- view count -->
        <div class="view-count section">
          <CustomText tag="b">1.673 like</CustomText>
        </div>
      <!-- comment list -->

      <!-- date time -->

      <!-- comment form -->


  </div>
</template>

<script>
import Avatar from "./Avatar";
import IconMore from "@/icons/more.svg"
import IconLike from "@/icons/like.svg"
import IconComment from "@/icons/comment.svg"
import IconDirect from "@/icons/direct.svg"
import IconSave from "@/icons/save.svg"
import CustomText from "@/components/CustomText";
export default {
  name: 'Post',
  components: {
    Avatar,
    CustomText,
    IconMore,
    IconLike,
    IconComment,
    IconDirect,
    IconSave,
  },
};
</script>

<style scoped>
.post{
  border-radius: 3px;
  border: 1px solid rgb(var(--b6a));
}
.section {
  padding-left: 16px;
  padding-right: 16px;
}
.header{
   height: 60px;
    display: flex;
    align-items: center;

  &-author {
     display: flex;
     align-items: center;

    &-info{
  margin-left: 8px;
     }
   }

   &-more {
    margin-left: auto;
    }
}
.action-buttons{
  height: 45px;
  display: flex;
  align-items: center;

    button {
    margin-right: 8px
    }

    .action-save{
      margin-left: auto;
      margin-right: 0;
    }
}
</style>