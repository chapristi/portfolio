<template>
  <section class="cardPresentation">
    <h1>Development Services</h1>
    <p class="text">
      Sample text. Click to select the text box. Click again or double click to
      start editing the text.
    </p>
    <article>
      <CustomCardService
        title="Development : "
        paragraph="Une architecture de projet minutieuse qui vous permet un maintient dans le temps peu coûteux mais aussi très simple. Notre  stratégie abordée a déjà porté ses fruits chez de nombreux clients"
        linkImage="https://cdn.discordapp.com/attachments/769652351333171250/1002955373436739664/app-development.png"
      />
      <CustomCardService
        title="Référencement :"
        paragraph="Nous vous aidons à référencer votre site internet grâce à un  code optimal  basé sur les règles de SEO et des recommandations données par Google."
        linkImage="https://cdn.discordapp.com/attachments/769652351333171250/1002957836906663946/world-wide-web_1.png"
      />
      <CustomCardService
        title="From scratch :"
        paragraph="Nous réalisons les sites internet à la main sur une base vierge afin d’obtenir un résultat le plus proche possible de la maquette fourni"
        linkImage="https://cdn.discordapp.com/attachments/769652351333171250/1003966598408843314/resultats.png"
      />
      <CustomCardService
        title="Optimisation : "
        paragraph="Un code optimisé car nous utilisons les technologies les plus performantes du marché. Cela permettra un rendu le plus rapide possible"
        linkImage="https://cdn.discordapp.com/attachments/769652351333171250/1003965994387120198/efficacite.png"
      />
      <CustomCardService
        title="support :"
        paragraph="24h/24 7j/7* Nous encourageons nos clients à  venir nous contacter s'ils rencontrent n’importe quel souci. Notre service client est compétent et sera capable de répondre à n'importe quelle de vos questions."
        linkImage="https://cdn.discordapp.com/attachments/769652351333171250/1003966349682429952/customer-service.png"
      />
      <CustomCardService
        title="La sécurité notre priorité: "
        paragraph="Grace au technologie utiliser ainsi qu'au code robuste, nous garantissons une protection contre des potentiels attaque * => voir pour plus d'information (et on dit que l'ont couvre uniquement les failles XSS - Injection SQL)"
        linkImage="https://cdn.discordapp.com/attachments/769652351333171250/1003965776493039687/cyber.png"
      />
    </article>
  </section>
  <section class="profilePresentation">
    <article class="picturePresentation">
      <CardViewProfile
        link="https://cdn.discordapp.com/attachments/767830436809801729/886181433947861022/20210911_112546.jpg"
      />
    </article>
    <article class="textPresentation">
      <div>
        <h2>
          Our management consulting services focus on our clients' most critical
          issues
        </h2>
        <p>
          I thought I had it figured out – I'd moved from Gujarat to Texas and
          was working with a trailblazing team at AT&T, literally one of the
          biggest companies in the world.
        </p>
        <p>
          Sem fringilla ut morbi tincidunt augue interdum velit. Nunc sed
          blandit libero volutpat sed cras. Risus quis varius quam quisque id.
          Semper auctor neque vitae tempus quam pellentesque nec nam aliquam. Et
          tortor consequat id porta nibh. Tincidunt id aliquet risus feugiat in
          ante metus dictum at. Feugiat pretium nibh ipsum consequat.
        </p>
        <a href="https://github.com/hyverno">read more</a>
      </div>
    </article>
  </section>
  <section class="questionsPresentation">
    <h1>We partner with the world's leading universities</h1>
    <div>
      <article class="questions-article">
        <suposedQuestions />
      </article>
      <article class="illustration-article">
        <img
          src="https://cdn.discordapp.com/attachments/769652351333171250/1003634058187767898/Untitled-2.png"
          alt="image de presentation"
        />
        <p class="textIllustration">
          Etiam erat velit scelerisque in dictum non consectetur. Nisl purus in
          mollis nunc sed id semper. Cras fermentum odio eu feugiat pretium nibh
          ipsum.
        </p>
      </article>
    </div>
  </section>
</template>
<style lang="scss">
body {
  margin: 0;
}
.cardPresentation {
  font-family: "Epilogue", sans-serif;
  width: 70%;
  margin: 0 auto;
  article {
    gap: 30px;
    flex-wrap: wrap;
    display: flex;
    justify-content: space-evenly;
  }
  .text {
    color: white;
    font-size: 20px;
  }
  h1 {
    font-size: 35px;
    color: #42b983;
  }
}
.profilePresentation {
  margin-top: 5%;
  width: 100%;
  display: flex;
  .textPresentation {
    width: 100%;
    text-align: left;
    div {
      padding-right: 25%;
      p {
        color: whitesmoke;
        font-size: 18px;
      }
      h2 {
        color: #42b983;
      }
    }
  }
  .picturePresentation {
    width: 100%;
  }
}
.questionsPresentation {
  width: 100%;
  height: 500px;

  h1 {
    color: #42b983;
    font-size: 35px;
    font-family: "Epilogue", sans-serif;
  }
  div {
    display: flex;
    height: 500px;
    .illustration-article {
      img {
        height: 70%;
        width: 70%;
        float: left;
      }
    }
    .textIllustration {
      font-size: 22px;
      float: left;
      text-align: left;
      padding-right: 30%;
    }
  }
  article {
    width: 100%;
  }
}
@media (max-width: 1237px) {
  .profilePresentation {
    display: flex;
    flex-direction: column;
    align-items: center;
    .textPresentation {
      div {
        padding-right: 10%;
        padding-left: 10%;
        text-align: center;
      }
    }
    .picturePresentation {
      .test {
        margin-right: auto;
        margin-left: auto;
      }
    }
  }
}
@media (max-width: 767px) {
  .questionsPresentation {
    width: 100%;
    height: 800px;

    div {
      display: flex;
      flex-direction: column;
      align-items: center;
      height: 700px;

      .questions-article {
        height: 300px;

        width: 100%;

        .question {
          height: 80%;
          margin-right: auto;
          margin-left: auto;
        }
      }
      .illustration-article {
        img {
          margin-left: 16%;
          height: 60%;
        }
        .textIllustration {
          padding-right: 15%;
          padding-left: 15%;
          text-align: center;
        }
      }
    }
  }
}
</style>

<script>
// @ is an alias to /src
import CustomCardService from "@/components/CustomCardService.vue";
import CardViewProfile from "@/components/CardViewProfile.vue";
import suposedQuestions from "@/components/suposedQuestions";

export default {
  data() {
    return {
      slides: [
        "https://picsum.photos/id/230/600/300",
        "https://picsum.photos/id/231/600/300",
      ],
    };
  },
  name: "HomeView",
  components: {
    CustomCardService,
    CardViewProfile,
    suposedQuestions,
  },
};
</script>
