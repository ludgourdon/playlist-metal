<template>
    <carousel :data="data" :autoplay="false" :interval="2147483647"></carousel>
</template>

<script>
  import Vue from 'vue';
  import VueCarousel from '@chenfengyuan/vue-carousel';
  Vue.component(VueCarousel.name, VueCarousel);

  export default {
    data() {
      return {
        data: [
            '<div class="example-slide first"><div class="first-comment">Salut à toi visiteur,' +
            '<br><br>Je te présente ma playlist Metal du moment. De l\'ancien au récent, tous styles confondus : death, black, doom,' +
            ' hardcore, tu découvriras une selection de morceaux que j\'apprécie le plus. Fais moi plaisir pour cette écoute ' +
            ' mets un casque ou utilises des enceintes qui envoient du lourd.' +
            '<br>Dès que tu es prêt cliques à droite.<br><br>Bonne écoute !</div></div>',
          '<div class="example-slide"><div class="comment">Commençons par un truc bien violent : Nails.<br>C\'est typiquement le truc ' +
          'où les gens te diront "c\'est que du bruit". Ouais ben allez y les gars, prenez les instruments ' +
          'essayez d\'envoyer ça et on en reparle. <br>Bon ok ils font pas dans la dentelle, c\'est ultra violent, mais ' +
          'devines quoi : c\'est le but recherché. Je crois qu\'on les qualifie de punk metal ' +
          'Dans leurs morceaux y\'a souvent ce truc typiques des groupes de punk hardcore avec  l\'alternance de rythmique bien rapide ' +
          'propre au punk et bim un break avec un gros groove lourd.' +
          'Je suis devenu fan de Nails. Vu au Hellfest, ils m\'ont cloué sur place.' +
          ' Je trouve qu\'ils maitrisent bien leur son pour un truc aussi bourrin et quand j\'écoute j\'ai ce ' +
          'truc un peu "poils qui s\'hérissent", c\'est un peu l\'exutoire de haine que j\'accumule.' +
          'Les morceaux sont courts, pas de chichi.</div>' +
          '<iframe width="960" height="540" src="https://www.youtube.com/embed/hGGGh03jN4w" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>',
          '<div class="example-slide">' +
          '<div class="comment">' +
           'Encore des ricains. Mais dans un tout autre registre : du stoner rock. Red Fang fait partie des inspirations d\'Idiocracy.' +
          'Ils ont des purs riffs, du rock\'n roll avec un bon son gras comme il faut. En plus le clip est plutôt marrant. Rien d\'autre à ajouter.'+
          '</div>' +
          '<iframe width="960" height="540" src="https://www.youtube.com/embed/VufilzHKTqk" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>' +
          '</div>',
          '<div class="example-slide">' +
          '<div class="comment">' +
          'Un petit tour chez les rosbeefs avec Conan.' +
          '<br>Haaaa Conan, encore de la finesse. Je pense que c\'est l\'un des groupes qui a les riffs les plus lourds que ' +
          'je connaisse. Je crois que le style c\'est du "battle doom". Les gars ils ont un accordage de guitare/basse débile, ' +
          'un accordage super grave, afin d\'avoir le son le plus' +
          ' lourd possible. C\'est presque une prouesse d\'arriver à faire sonner son instrument avec un accordage si grave, à ce stade' +
          ' tes cordes ce sont des spaghettis normalement. Conan c\'est pas toujours super original, ils se répètent un peu, riffs ultra lourds,' +
          'souvent lent, un gars qui gueule du fond des bois. Mais j\'adore ce morceau, bien puissant et je viens de trouver ce montage video' +
          'qui pour le coup colle plutot bien au morceau et à l\'univers du groupe qui je pense est de toutes façons inspiré par l\'univers de ' +
          'Conan le Barbare. Me dis pas que quand t\'écoutes ça t\'as pas envie de monter une armée d\'orques et d\'aller tout anéantir !' +
          '</div>' +
          '<iframe width="960" height="540" src="https://www.youtube.com/embed/iMZ2-xBjsRY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>' +
          '</div>',
            '<div class="example-slide">' +
            '<div class="comment">' +
            'Un truc un peu plus gayzou maintenant. Pain of salvation c\'est un groupe un peu chelou, ils font une sorte de metal prog, avec des influences ' +
            'un peu diverses, rock, pop, folk. J\'aime pas tout mais ils ont des bons trucs. En tout cas je kiffe ce morceau.' +
            '</div>' +
            '<iframe width="960" height="540" src="https://www.youtube.com/embed/MreXYqelGPM" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>' +
            '</div>',
            '<div class="example-slide">' +
            '<div class="comment">' +
            'Alors je sais pas si t\'as suivi l\'évolution de Septicflesh, mais les mecs ils ont plutôt très bien évolué.' +
            'Globalement leur 4 derniers albums sont vraiment pas mal. Je crois que les premières écoutes de Septicflesh devaient ' +
            'être à la fin des 90s, grâce aux CDS qu\'on se faisait livrer par adipocere, holy records (quelle époque !). ' +
            'Et Septic flesh c\'était pas mal mais bon on était un peu Septicflesh quand même. Ben les gars ils ont sortis ' +
            'l\'artillerie lourde avec des orchestrations, des riffs bien puissants, ça fait plaisir un groupe qui a su garder ' +
            'des orchestrations et des trucs mélodiques en gardant un côté dark et puissant, sans tomber dans des trucs heavy relou ' +
            'avec des reprises de poupées de cire/poupéé de son... si vous voyez ce que je veux dire...' +
            '</div>' +
            '<iframe width="960" height="540" src="https://www.youtube.com/embed/MfoJIe3MDBY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>'+
            '</div>',
        ],
      };
    },
  };
</script>

<style>
    .example-slide {
        align-items: center;
        background-color: #000;
        color: #999;
        display: flex;
        font-size: 1rem;
        justify-content: center;
        min-height: 10rem;
        height: 90vh;
        padding: 0 5vw;
    }

    .first {
        font-size: 1.5rem;
    }

    .first-comment {
        width:80%;
    }

    .comment {
        width:25%;
        padding-right:10px;
    }
</style>
