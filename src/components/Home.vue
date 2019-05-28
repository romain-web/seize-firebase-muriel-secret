<template>
  <div class="home">
    <section>
      <figure>
        <a href="https://www.seize.tv/les-secrets-de-muriel" class="nostyle">
          <img alt="background header" src="../assets/live.png" />
        </a>
      </figure>
    </section>

    <div class="cards">
      <section>
        <div class="card">
          <h3>Biscuit moelleux noix de pécans :</h3>
          <ul>
            <li>1 œufs</li>
            <li>75 g de cassonade</li>
            <li>1 pincée de sel</li>
            <li>35 g de farine</li>
            <li>2 g de levure chimique</li>
            <li>2 blancs d'oeufs</li>
            <li>15 g de cassonade</li>
            <li>70 g de beurre doux</li>
            <li>75 g de noix de pécan</li>
          </ul>
        </div>
        
        <div class="card">
          <h3>Confit exotique :</h3>
          <ul>
            <li>110 g de purée de fruits de la passion</li>
            <li>1 mangue</li>
            <li>1 petite banane mûre</li>
            <li>1 ananas Victoria</li>
            <li>1 citron vert</li>
            <li>30 g de sucre semoule</li>
            <li>6 g de pectine NH (attention, pas de pectine à confiture) se trouve chez Zodio, magasin spécialisés ou sur internet. Si vraiment pas je vous donnerai un équivalent avec du agar ou de la gélatine (bien moins bon en texture).</li>
          </ul>
        </div>

        <div class="card">
          <h3>Mousse érable :</h3>
          <ul>
            <li>190 g de crème liquide 35% (sinon 30% min. avec mascarpone)</li>
            <li>55 g lait entier</li>
            <li>1 gousse de vanille</li>
            <li>3 g gélatine (qualité or ou 200 Bloom) Vous pouvez la trouvez en supermarché mais il faudra bien faire attention au pouvoir gélifiant. Muriel vous donnera en live les conseils pour adapter le dosage.</li>
            <li>55 g crème liquide entière</attention>
            <li>100 g de sirop d'érable</li>
            <li>1 blanc d'oeuf</li>
          </ul>
        </div>

        <div class="card">
          <h3>Glaçage rapide :</h3>
          <ul>
            <li>150 g crème liquide 35%</li>
            <li>1,5 g de gélatine or</li>
            <li>150 g crème liquide 35 % (ou 30% avec mascarpone)</li>
          </ul>
        </div>
      </section>
    </div>

    <section class="text-center">
      <h2>Pour les plus courageux du chocolat blanc pour faire des décors !</h2>
    </section>

    <section class="bottom mrg-top-lg">
      <h2>Pour aller un peu plus loin :</h2>

      <ul>
        <li>Pour voir l’esprit de la bûche… en un peu plus compliqué <a href="https://youtu.be/iSBgHDWwiX4" target="_blank" rel="noopener noreferrer">https://youtu.be/iSBgHDWwiX4</a></li>

        <li>Pour trouver le moule à bûche de Buyer avec les feuilles texturées rendez- vous sur leur site <a href="https://www.debuyer.com/fr/boutiques-en-france" target="_blank" rel="noopener noreferrer">www.debuyer.com</a></li>

        <li>Vous trouverez le moule à bûche en inox et le set de 4 feuilles texturées aussi chez la merveilleuse Sandrine de Cuisineshop : <a href="https://www.cuisineshop.fr/" target="_blank" rel="noopener noreferrer">www.cuisineshop.fr</a></li>

        <li>Mais aussi l'élastomoule demi sphère 48 pcs DE BUYER  et le cadre extensible tout inox DE BUYER sur <a href="https://www.francisbatt.com/" target="_blank" rel="noopener noreferrer">www.francisbatt.com</a></li>
      </ul>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Home',
  props: {
    msg: String
  }
}
</script>

<style lang="scss">
@import '~@/assets/style/variables';

.home {
  figure {
    width: 100%;
    margin: auto;
    text-align: center;

    img {
      max-width: 1000px;
      width: 100%;
    }
  }

  section {
    max-width: 1200px;
    margin: auto;
  }

  ul {
    list-style: circle;
    li {
      line-height: 1.5rem;
      margin-bottom: $gutter-sm;
    }
  }

  @media screen and (max-width: 1200px) {
    .bottom {
      padding: 0 $gutter-md;
    }
  }

  .cards {
    > section {
      padding: $gutter-sm;
      @media screen and (min-width: 420px) {
        padding: $gutter-lg;
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
      }
    }
    margin-bottom: $gutter-md;
    background: url('~@/assets/restaurant_icons.png');
  }

  .card {
    // @include card(1);
    border-radius: $gutter;
    width: auto;
    background: $white;
    border: 1px solid $palette-grey-100;

    margin: $gutter-sm;
    padding: $gutter-md;
    @media screen and (min-width: 420px) {
      width: 280px;
      margin: $gutter-md;
      padding: $gutter-md;
    }
  }
}
</style>
