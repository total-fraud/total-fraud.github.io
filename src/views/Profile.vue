<template>
  <div class="Profile-container">
    <Header />
    <section class="profile">
      <div class="profile__avatar">
        <img class="avatar" src="@/assets/profile-pic.jpg" alt="profile pic" />
      </div>
      <div class="profile__info">
        <div class="name-and-btns">
          <span class="nickname">total_fraud</span
          ><button class="profile__edit">Edit Profile</button>
        </div>
        <div class="profile__numbers">
          <a class="post-numbers numbers-padding">20 posts</a>
          <a class="followers-numbers numbers-padding">48 followers</a>
          <a class="following-nubers">120 follow</a>
        </div>
        <div class="profile__description">
          <span class="userName">userName</span
          ><span class="profile__about">just ordinary man</span>
        </div>
      </div>
    </section>
    <section class="gallery">
      <figure class="gallery-item">
        <img
          src="https://picsum.photos/500/500"
          class="gallery-img"
          alt="Image 1"
        />
      </figure>
      <figure class="gallery-item">
        <img
          src="https://picsum.photos/500/500"
          class="gallery-img"
          alt="Image 2"
        />
      </figure>
      <figure class="gallery-item">
        <img
          src="https://picsum.photos/500/500"
          class="gallery-img"
          alt="Image 3"
        />
      </figure>
      <figure class="gallery-item">
        <img
          src="https://picsum.photos/500/500"
          class="gallery-img"
          alt="Image 4"
        />
      </figure>
      <figure class="gallery-item">
        <img
          src="https://picsum.photos/500/500"
          class="gallery-img"
          alt="Image 5"
        />
      </figure>
      <figure class="gallery-item">
        <img
          src="https://picsum.photos/500/500"
          class="gallery-img"
          alt="Image 6"
        />
      </figure>
    </section>
  </div>
</template>

<script>
import Header from "@/components/Header";

export default {
  components: {
    Header
  }
};
</script>

<style scoped>
.Profile-container {
  background-color: #f2f2f2;
  display: grid;
  grid-template-columns: 1fr minmax(auto, 900px) 1fr;
  grid-template-rows: 54px auto 1fr;
  grid-column-gap: 0;
  grid-template-areas:
    "header header header"
    ".      profile     ."
    ".      gallery     .";
}
.profile {
  padding: 30px 0;
  grid-area: profile;
  display: flex;
}

.profile__avatar {
  width: 350px;
  height: 150px;
  border-radius: 50%;
  text-align: center;
  padding-right: 50px;
}
.avatar {
  height: 150px;
  width: 150px;
  border-radius: 50%;
}

.profile__info {
  display: flex;
  flex-flow: column nowrap;
  align-items: flex-start;
}
.name-and-btns {
  display: flex;
  justify-content: flex-start;
}
.nickname {
  color: #262626;
  font-family: "Oswald", sans-serif;
  font-weight: 400;
  font-size: 22px;
  text-decoration: none;
  padding-right: 15px;
}

.profile__edit {
  background-color: transparent;
  border-radius: 4px;
  height: 30px;
  cursor: pointer;
  color: #262626;
  font-family: "Roboto", sans-serif;
  font-size: 0.8em;
  font-weight: 500;
  line-height: 0.8;
  padding: 4px 9px;
  border: 1px solid #dbdbdb;
}

.profile__numbers {
  padding-top: 15px;
  cursor: pointer;
  color: #262626;
  font-family: "Roboto", sans-serif;
  font-size: 0.9em;
  font-weight: 500;
}

.post-numbers,
.numbers-padding,
.following-nubers {
  cursor: pointer;
}
.numbers-padding {
  padding-right: 8px;
}

.profile__description {
  margin-top: 15px;
  display: flex;
  flex-flow: column nowrap;
}
.userName {
  color: #262626;
  font-family: "Oswald", sans-serif;
  font-weight: 400;
  font-size: 18px;
  text-decoration: none;
  padding-right: 15px;
}
.profile__about {
  color: #262626;
  font-family: "Roboto", sans-serif;
  font-size: 0.9em;
  font-weight: 500;
}
.gallery {
  grid-area: gallery;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  grid-gap: 20px;
  align-items: stretch;
}

.gallery-img {
  border: none;
  box-shadow: 2px 2px 6px 0px rgba(0, 0, 0, 0.3);
  max-width: 100%;
}
</style>
