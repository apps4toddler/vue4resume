<template>
  <section class="about">
    <h3 class="visually-hidden">About</h3>
    <picture><img src="@/assets/img/profile.png" alt="photo of takuya" class="photo" /></picture>
    <p>
      <span class="welcome">&lt;Hello, world! /&gt;</span>
      <span class="text">
        My name is
        <span class="primary"> Takuya Sato</span>
        and I'm 
        <span class="primary"> world class digital transformation partner</span>
        for business owners solving social challenge.
      </span>  
      <span class="text">
        I definity believe that the future will be a wonderful world with digital innovation.
      </span>  
      <span class="text">
        My mission is technology innovation for this earth, so I'm going to provide leadership in emerging technology all over the world.
      </span>  
      <span class="text">
        And now I try not to dwell on what I've already achieved, therefore I'm constantly learning something new in order to further develop in the closen path.
      </span>  
      <span class="text">
        At the moment I'm interested in:
      </span>  
      <span class="text">
        <span class="stack">
          <span class="icon tip iconsize">
            <img src="@/assets/png/icon-flutter.svg.png">
            <span class="title">Flutter</span>
          </span>
          <span class="icon tip iconsize">
            <img src="@/assets/png/icon-dart.svg.png">
            <span class="title">Dart</span>
          </span>
          <span class="icon tip iconsize">
            <img src="@/assets/png/icon-kotlin.svg.png">
            <span class="title">Kotlin</span>
          </span>
        </span>
      </span>  
    </p>
  </section>
</template>

<script setup></script>

<style type="scss" scoped>

.tip {
  position: relative;
}

.tip .title {
  position: absolute;
  left: 50%;
  bottom: -100%; /* Y軸の位置 */
  transform: translateX(-50%);
  margin-bottom: 8px; /* テキストとの距離 */
  padding: 4px;
  border-radius: 10px; /* 角の丸み */
  background-color: #eee;
  font-size: 0.75em;
  color: #333;
  text-align: center;
  visibility: hidden; /* ツールチップを非表示に */
  opacity: 0; /* 不透明度を0％に */
  z-index: 1;
}


.tip:hover .title { /* マウスオーバー時のスタイル */
  bottom: -150%; /* Y軸の位置 */
  visibility: visible; /* ツールチップを表示 */
  opacity: 1; /* 不透明度を100％に */
}

.stack .icon {
  display: block;
}

.stack  .iconsize {
  width: 1.5rem;
  height: 1.5rem;
}

.stack .icon img {
  display:block;
  width: 100%;
  height: 100%;
}

.stack {
  display: grid;
  grid-column-gap: var(--space-4);
  grid-row-gap: var(--space-4);
  justify-self: center;

  grid-template-columns: repeat(auto-fill, minmax(1.5rem, 1fr));
  margin-top: var(--space-4);
}

.primary {
  color: var(--primary-500);
}
.text {
  display:block;
  margin-top: var(--space-4);
}
.welcome {
  color: var(--primary-400);
  font-weight: 600;
}
.photo {
  min-width:16rem;
  height: 16rem;
  float: none;
  margin-right: var(--space-6);
  margin-bottom: var(--space-6);
  width: 8rem;
}

.about {
  display: flex;
  margin-right: var(--space-6);
  margin-bottom: var(--space-6);
  margin-left: var(--space-6);

  border:1px solid #ccc;
}

</style>

