<template>
  <div class="c-ethnic-cossacks">
    <h2 class="title">Этническое казачество</h2>
    <div class="cards-list__wrapper">
      <c-card-1 v-for="product in products" :key="product.article" :product_data="product" />
    </div>
  </div>
</template>

<script>
import cCard1 from './c-card-1';

export default {
  name: 'c-ethnic-cossacks',
  components: {
    cCard1,
  },
  props: {},
  data() {
    return {
      products: [
        {
          image: '1.jpg',
          name: 'T-shirt 1',
          description: 'alfkbalkf blakfj blakefj kaefj ka;efj lkaejf aejfalvkejrgljqerijvnqerkj nqer qejr iqjern kjqer kjqerljblkqjerk jqnelkrj lqejrn klkjqenr ',
          article: 'T1',
          available: true,
          category: 'Мужские',
        },
        {
          image: '2.jpg',
          name: 'T-shirt 2',
          description: 'ajwbhvljaervbjhaevlaeff ijieq iqepiurb iqerpiu uqeij jpiqeunr piqe tpiuqeijn pqitet ipqepifjj qpien iqebr ipuqpeiru pique piuqet ',
          article: 'T2',
          available: true,
          category: 'Женские',
        },
        {
          image: '3.jpg',
          name: 'T-shirt 3',
          description: 'ajehbvaojhb qeripqerjn piqueiru k jenflh baehfn kjqebruin qeirb iuqennripubvqepruoqer iuqen[ori q]peorn iuqebr[o iubqeiru ]',
          article: 'T3',
          available: false,
          category: 'Женские',
        },
        {
          image: '4.jpg',
          name: 'T-shirt 4',
          description: 'kajdbvlKD LKABDFL KJBBEFALKJ BQKER LBEKR;kjndf;kj nd;ksgjn ;kjasgn ;kjN;JN ;KJANGT;KJ nfljknkrjbtkb',
          article: 'T4',
          available: true,
          category: 'Мужские',
        },
        {
          image: '5.jpg',
          name: 'T-shirt 5',
          description: 'akkejrbnakerkaer iiqerihb qerri qberrb kqjerrkl bq;ekrjblkqjernbkjefrvbkljqbe;kjrvblqkjernvb;kjqerrk; erqlk bqkljern kljqe lkqebtk jqbekjr lkqjebr kqebr lkjqe;rkj blqkjebf jlqkenr kljqjer kjqerk j',
          article: 'T5',
          available: false,
          category: 'Женские',
        },
        {
          image: '6.jpg',
          name: 'T-shirt 6',
          description: 'lAKJDBVKjjfb j EFL HEIHRB IQEBFB JKkj;jbr krjgn kdgf kladffk bdfj a kljetbjqenriuvbhqkjrevbkjasbv man sdknefkl bqer ihqer iqebir bqerib kpqerj kqerjrb piqerjhipuuhqieuv qjneiuru ipuqebr iupqerhi ubqiepuru ipuhewipu hqipuer',
          article: 'T6',
          available: true,
          category: 'Женские',
        },
      ],
    };
  },
};
</script>

<style>
.cards-list__wrapper {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 20px;
}
</style>
