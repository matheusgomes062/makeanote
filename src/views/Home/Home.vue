<template>
  <div id="main">
    <div id="aboutContainer">
      <div id="imgContainer">
        <img src="https://media-exp1.licdn.com/dms/image/C4E03AQHD2VTOY5tyQA/profile-displayphoto-shrink_200_200/0/1602727285269?e=1612396800&v=beta&t=1lLXvOT1lF66aFyQWlNJzYQPkReIBMcrVtvsf-0LNv8" alt="profile-picture">
      </div>
      <div id="aboutSection">
        <section>
          <h2>Sobre</h2>
          <p v-html="about"/>
        </section>
        <section>
          <h2>Objetivo</h2>
          <p v-html="objective"/>
        </section>
      </div>
    </div>
    <div id="quickInfo">
      <table>
        <tr>
          <th v-for="column in tableTitles" :key="column">{{ column }}</th>
        </tr>
        <tr>
          <td v-for="row in formations" :key="row">
            <ul>
              <li>
                {{ row }}
              </li>
            </ul>
          </td>
        </tr>
        <tr>
          <td v-for="row in qualifications" :key="row">
            <ul>
              <li>
                {{ row }}
              </li>
            </ul>
          </td>
        </tr>
        <tr>
          <td v-for="row in experiences" :key="row">
            <ul>
              <li>
                {{ row }}
              </li>
            </ul>
          </td>
        </tr>
      </table>
    </div>
  </div>
</template>

<script>
export default {
  name: "home",
  props: {
  },
  components: {
  },
  data() {
    return {
      about: "Trabalho como desenvolvedor Full Stack desde 2018 e atualmente estou me aprofundando em desenvolvimento web, .NET e DDD + Clean Code.<br/>Tenho familiaridade com as principais linguagens de programação web (HTML, CSS e JavaScript), além de possuir conhecimentos em API e Banco de Dados, utilizando ferramentas, como JQuery, PostgreSQL, SQL Server Manager e SQLite.<br/>Possuo também experiência em, linguagem C, C#, Git, SPA, SASS, Vuejs e mais recentemente React e React-Native. Além de ter cursos de SCRUM, Design Thinking, Inteligência Artificial e Web Design.<br/>Já escrevi durante quase um ano para um site de notícias relacionadas a Blockchain e Criptomoedas e contribuo ativamente para o dev.to, onde já consegui impactar mais de 17 mil pessoas com meus posts. Também fui membro, monitor e professor da área de Criatividade do Centro de Estudos em Games e Internet na UNIFESP.<br/>Por fim, sou viciado em trabalho, empreendedorismo e hackathons, sobre este último já participei de alguns e minha melhor posição foi quarto lugar na américa latina e segundo lugar no Brasil!",

      objective: "Um dia trabalhar numa empresa FANG (Facebook, Amazon, Netflix, Google), ou viajar pelo mundo gerindo minha própria empresa!",

      tableTitles: ["Formação", "Qualificação Técnica", "Experiências Profissinais"],

      formations: [
        "Ensino Médio Completo",
        "Licenciatura em Matemática incompleto", 
        "Bacharelado em Ciência e Tecnologia em curso"],
        
      qualifications: [
        "VueJs", 
        "ReactJs",
        ".NET Core"],

      experiences: [
        "Redator Conteúdo Web",
        "Full Stack Developer - Agrotools",
        "Full Stack Engineer - Ânima Educação"],
    };
  },
  mounted() {
  },
  methods: {
  }
};
</script>

<style lang="scss" scoped>
    @import "./home.scss";
</style>