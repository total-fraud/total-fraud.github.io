<template>
  <article class="post">
    <header class="post__header">
      <a class="op" href>
        <svg
          version="1.1"
          class="op__icon"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          x="0px"
          y="0px"
          viewBox="0 0 1000 1000"
          enable-background="new 0 0 1000 1000"
          xml:space="preserve"
        >
          <g>
            <g
              transform="translate(0.000000,512.000000) scale(0.100000,-0.100000)"
            >
              <path
                d="M4622.6,5016.9c-693.8-70.9-1213.2-214.7-1782.4-494.5c-500.2-245.3-856.7-498.3-1263-891.2c-417.8-408.2-722.6-828-981.3-1353.1c-241.5-494.5-389.1-979.4-471.5-1552.4c-32.6-226.2-32.6-981.3,0-1207.5c136.1-950.6,504.1-1803.5,1082.9-2506.9c1353.1-1642.5,3595.5-2229,5571.5-1458.5C8043.7-3952.7,9071-2923.5,9569.3-1650.9C9772.5-1127.7,9876-625.6,9897-41c46,1326.3-446.6,2604.6-1374.2,3562.9c-421.7,435.1-833.7,736-1370.4,998.5c-483,237.7-927.6,377.6-1466.2,460C5492.8,5009.2,4789.4,5034.1,4622.6,5016.9z M5638.4,4675.7c994.7-147.6,1908.9-605.6,2608.4-1307.1c724.5-728.3,1169.1-1631,1314.8-2671.7c36.4-266.4,30.7-952.6-9.6-1217c-118.8-772.4-417.8-1496.8-866.3-2096.7c-74.8-101.6-176.3-226.2-226.2-279.8l-88.2-95.8l-21.1,63.2c-103.5,289.4-316.2,619.1-569.2,885.5c-529,555.8-1218.9,893.1-2104.4,1027.3c-322,49.8-1038.8,49.8-1360.8,0c-833.7-126.5-1475.8-421.6-1997.1-918C2209.7-2040,2064-2201,1995-2291.1c-115-155.3-297.1-483-350.7-634.4l-23-67.1l-88.2,95.8c-49.8,53.7-151.4,178.2-226.2,279.8C421.5-1432.4,164.7,120,618.9,1526.8c458,1412.5,1562,2516.5,2976.4,2972.6c322,105.4,594.1,159.1,1056,210.8C4791.3,4725.5,5454.4,4702.5,5638.4,4675.7z"
              ></path>
              <path
                d="M4651.4,3228.7c-197.4-42.2-385.2-115-565.4-220.4c-185.9-109.2-473.4-398.7-588.4-596.1c-341.1-580.7-322-1295.6,53.7-1861c329.6-498.3,918-795.4,1512.2-768.6c268.3,13.4,465.7,65.2,709.1,184c341.1,168.7,609.5,437,778.1,778.1c141.8,287.5,176.3,440.8,176.3,776.2c0,327.7-34.5,483-166.7,757C6213.4,2994.9,5419.9,3389.7,4651.4,3228.7z"
              ></path>
            </g>
          </g>
        </svg>
      </a>
      <div class="op__name profile-name">{{ post.name }}</div>
      <button type="button" class="post__func-btn">
        <svg
          version="1.1"
          class="op__icon_func-btn"
          xmlns="http://www.w3.org/2000/svg"
          xmlns:xlink="http://www.w3.org/1999/xlink"
          x="0px"
          y="0px"
          viewBox="0 0 32.055 32.055"
          style="enable-background:new 0 0 32.055 32.055;"
          xml:space="preserve"
        >
          <g>
            <path
              d="M3.968,12.061C1.775,12.061,0,13.835,0,16.027c0,2.192,1.773,3.967,3.968,3.967c2.189,0,3.966-1.772,3.966-3.967
		C7.934,13.835,6.157,12.061,3.968,12.061z M16.233,12.061c-2.188,0-3.968,1.773-3.968,3.965c0,2.192,1.778,3.967,3.968,3.967
		s3.97-1.772,3.97-3.967C20.201,13.835,18.423,12.061,16.233,12.061z M28.09,12.061c-2.192,0-3.969,1.774-3.969,3.967
		c0,2.19,1.774,3.965,3.969,3.965c2.188,0,3.965-1.772,3.965-3.965S30.278,12.061,28.09,12.061z"
            ></path>
          </g>
        </svg>
      </button>
    </header>
    <div class="pic">
      <img class="post__pic" v-bind:src="post.content" alt="post" />
    </div>
    <div class="post__interact">
      <div class="post__btns">
        <button class="post__btn">
          <svg
            version="1.1"
            class="btn-pic"
            xmlns="http://www.w3.org/2000/svg"
            xmlns:xlink="http://www.w3.org/1999/xlink"
            x="0px"
            y="0px"
            viewBox="0 0 471.701 471.701"
            style="enable-background:new 0 0 471.701 471.701;"
            xml:space="preserve"
          >
            <path
              d="M433.601,67.001c-24.7-24.7-57.4-38.2-92.3-38.2s-67.7,13.6-92.4,38.3l-12.9,12.9l-13.1-13.1
		c-24.7-24.7-57.6-38.4-92.5-38.4c-34.8,0-67.6,13.6-92.2,38.2c-24.7,24.7-38.3,57.5-38.2,92.4c0,34.9,13.7,67.6,38.4,92.3
		l187.8,187.8c2.6,2.6,6.1,4,9.5,4c3.4,0,6.9-1.3,9.5-3.9l188.2-187.5c24.7-24.7,38.3-57.5,38.3-92.4
		C471.801,124.501,458.301,91.701,433.601,67.001z M414.401,232.701l-178.7,178l-178.3-178.3c-19.6-19.6-30.4-45.6-30.4-73.3
		s10.7-53.7,30.3-73.2c19.5-19.5,45.5-30.3,73.1-30.3c27.7,0,53.8,10.8,73.4,30.4l22.6,22.6c5.3,5.3,13.8,5.3,19.1,0l22.4-22.4
		c19.6-19.6,45.7-30.4,73.3-30.4c27.6,0,53.6,10.8,73.2,30.3c19.6,19.6,30.3,45.6,30.3,73.3
		C444.801,187.101,434.001,213.101,414.401,232.701z"
            ></path>
          </svg>
        </button>
        <button class="post__btn">
          <svg
            class="btn-pic"
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
          >
            <path
              d="M7 11c-.828 0-1.5-.671-1.5-1.5s.672-1.5 1.5-1.5c.829 0 1.5.671 1.5 1.5s-.671 1.5-1.5 1.5zm5 0c-.828 0-1.5-.671-1.5-1.5s.672-1.5 1.5-1.5c.829 0 1.5.671 1.5 1.5s-.671 1.5-1.5 1.5zm5 0c-.828 0-1.5-.671-1.5-1.5s.672-1.5 1.5-1.5c.829 0 1.5.671 1.5 1.5s-.671 1.5-1.5 1.5zm5-8v13h-11.643l-4.357 3.105v-3.105h-4v-13h20zm2-2h-24v16.981h4v5.019l7-5.019h13v-16.981z"
            ></path>
          </svg>
        </button>
        <button class="post__btn">
          <svg
            version="1.1"
            class="btn-pic"
            xmlns="http://www.w3.org/2000/svg"
            xmlns:xlink="http://www.w3.org/1999/xlink"
            x="0px"
            y="0px"
            viewBox="0 0 469.038 469.038"
            style="enable-background:new 0 0 469.038 469.038;"
            xml:space="preserve"
          >
            <g>
              <path
                d="M465.023,4.079c-3.9-3.9-9.9-5-14.9-2.8l-442,193.7c-4.7,2.1-7.8,6.6-8.1,11.7s2.4,9.9,6.8,12.4l154.1,87.4l91.5,155.7
		c2.4,4.1,6.9,6.7,11.6,6.7c0.3,0,0.5,0,0.8,0c5.1-0.3,9.5-3.4,11.6-8.1l191.5-441.8C470.123,13.879,469.023,7.979,465.023,4.079z
		 M394.723,54.979l-226.2,224.7l-124.9-70.8L394.723,54.979z M262.223,425.579l-74.5-126.9l227.5-226L262.223,425.579z"
              ></path>
            </g>
          </svg>
        </button>
        <button class="post__btn post__btn_right-position">
          <svg
            fill="#000000"
            class="btn-pic"
            xmlns="http://www.w3.org/2000/svg"
            viewBox="0 0 24 24"
            width="24px"
            height="24px"
          >
            <path
              d="M 6.0097656 2 C 4.9143111 2 4.0097656 2.9025988 4.0097656 3.9980469 L 4 22 L 12 19 L 20 22 L 20 20.556641 L 20 4 C 20 2.9069372 19.093063 2 18 2 L 6.0097656 2 z M 6.0097656 4 L 18 4 L 18 19.113281 L 12 16.863281 L 6.0019531 19.113281 L 6.0097656 4 z"
            ></path>
          </svg>
        </button>
      </div>

      <section class="comment-section">
        <span class="like-number">{{ post.likes }} likes</span>
        <ul class="comments-list">
          <li
            class="comments-item"
            v-for="comment in post.comments"
            v-bind:key="comment.id"
          >
            <a href class="comment-name">{{ comment.name }}</a>
            <span class="comment-text">{{ comment.text }}</span>
          </li>
        </ul>
        <section class="comment-section__post">
          <form action class="post-form">
            <input
              type="text"
              class="post-form__input"
              placeholder="Add a comment..."
            />
          </form>
        </section>
      </section>
    </div>
  </article>
</template>

<script>
export default {
  props: ["post"]
};
</script>

<style scoped>
.post {
  background-color: white;
  border-radius: 10px;
  margin-top: 30px;
}

.post__header {
  display: flex;
  flex-wrap: nowrap;
  justify-content: flex-start;
  flex-direction: row;
  align-items: center;
  height: 60px;
  padding: 10px;
  margin: 0;
  border-bottom: 1px solid #dbdbdb;
}

.op__icon {
  height: 28px;
  width: 28px;
}

.op__name {
  text-decoration: none;
  color: #262626;
  font-family: "Oswald", sans-serif;
  font-weight: 600;
  font-size: 0.8em;
  padding: 10px;
  width: 300px;
}

.post__func-btn {
  margin-left: auto;
  margin-right: 15px;
  padding: 0;
  border: none;
  background: none;
  cursor: pointer;
}

.op__icon_func-btn {
  width: 16px;
  height: 16px;
}

.post__pic {
  width: 100%;
  max-width: 600px;
  max-height: 600px;
}

.post__interact {
  height: 100%;
}

.post__btns {
  display: flex;
}

.post__btn {
  padding: 8px 8px 8px 12px;
  border: none;
  background: none;
  cursor: pointer;
}

.post__btn:last-child {
  margin-left: auto;
}

.btn-pic {
  height: 24px;
  width: 24px;
}

.comment-section {
  display: flex;
  flex-flow: column nowrap;
}

.like-number {
  color: #262626;
  font-family: "Oswald", sans-serif;
  font-weight: 600;
  font-size: 0.8em;
  padding-left: 12px;
  padding-bottom: 2px;
}

.comments-list {
  list-style: none;
  margin-bottom: 5px;
  padding-left: 12px;
}

.comment-name {
  color: #262626;
  font-family: "Oswald", sans-serif;
  font-weight: 600;
  font-size: 0.8em;
  text-decoration: none;
}

.comment-text {
  color: #262626;
  font-family: "Oswald", sans-serif;
  font-weight: 400;
  font-size: 0.8em;
  padding-left: 7px;
}

.post-form {
  margin-top: 8px;
  padding-left: 0px;
  margin-bottom: 8px;
}

.post-form__input {
  padding-left: 12px;
  padding-top: 3px;
  padding-bottom: 3px;
  width: 100%;
  border: none;
  border-top: 1px solid #dbdbdb;
}
</style>
