<template>
  <div class="landing-page" vocab="https://schema.org/" typeof="WebPage">
    <div class="hero-section">
      <img class="hero-image" src="@/assets/images/hero.jpg" alt="Finnish Spitz" property="primaryImageOfPage" />
      <h1 class="hero-title" property="name">Finnish Spitz</h1>
      <h2 class="hero-subtitle">The Friendly and Lively National Dog of Finland</h2>
    </div>
    <div class="content-section" typeof="Thing">
      <p property="description">
        The Finnish Spitz, also known as Suomenpystykorva or Finsk Spets, is a breed of dog that originated in Finland.
        They are the national dog of Finland and have a long history as hunting and companion animals. Finnish Spitz
        dogs are known for their intelligence, agility, and friendly temperament, making them great family pets.
      </p>
      <p>
        With their beautiful red-gold coat, the Finnish Spitz is an attractive and eye-catching breed. Their fox-like
        appearance is further accentuated by their pointed ears and curled tail. Despite their small size, they are
        sturdy and well-suited for various activities, including hunting, agility, and obedience training.
      </p>
      <p>
        Finnish Spitz dogs are affectionate and social creatures, making them perfect companions for families, singles,
        and seniors alike. Their loyalty and devotion to their owners make them excellent watchdogs. They are also
        good with children and other pets, although early socialization is essential.
      </p>
    </div>
    <a href="/imt-doggos/about-finnish-dogs">Learn more about Finnish dogs, specifically the Finnish Spitz</a>
  </div>
</template>

<script lang="ts">
export const documentProps = {
  title: "The Finnish Spitz",
  description: "Learn about the Finnish Spitz, the national dog of Finland. Discover its distinctive look, temperament, training needs, and care tips. The page also features a user-based rating of the breed."
};
export default {}
</script>

<style scoped>
.landing-page {
  display: flex;
  flex-direction: column;
  align-items: center;
  font-family: Arial, sans-serif;
}

.hero-section {
  position: relative;
  text-align: center;
  margin-bottom: 2rem;
}

.hero-image {
  width: 100%;
  height: auto;
  object-fit: cover;
}

.hero-title {
  font-size: 3rem;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: white;
  text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.6);
  padding: 32px 0;
  width: 100%;
  background: rgba(0, 0, 0, 0.5);
}

.hero-subtitle {
  font-size: 1.5rem;
  color: orangered;
  text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.6);
}

.content-section {
  max-width: 900px;
  text-align: justify;
  line-height: 1.5;
  padding: 0 1rem;
}
</style>
