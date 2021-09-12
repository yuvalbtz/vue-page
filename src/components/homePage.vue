<template >

<v-container v-bind:style="styleObject" >
    <v-row align="center"  justify="center"
      >
     <v-col justify="center" class="text-center" >
        <h1 style="color:white" class="display-2 font-weight-bold mt-7"
        >
       מותאמת אישית Bootcamp תוכנית
        </h1>
     <h1 style="color:white" class="display-0 font-weight-bold mt-3"
        >
      להפוך למתכנת בהייטק בליווי אישי + סטאז׳ תוך 3 חודשים
       בשילוב קאוצ׳ינג אישי ועבודת צוות
     <h6>{גם אין לך רקע או ניסיון בתחום בכלל}</h6> 
        </h1>
         </v-col>
</v-row>



<v-row class="mt-3" align="center"  justify="center" >
    <v-btn
  color="primary"
  elevation="7"
  outlined
  raised
  x-large
  class="mr-5"
>
דברו איתנו
</v-btn>
   
    <v-btn
  color="primary"
  elevation="7"
  outlined
  raised
  x-large
  
>
פרטים נוספים
</v-btn>
</v-row>

<v-row align="center"  justify="center" class="mt-10" >
  <a>
    <svg style="width:64  px;height:64px" viewBox="0 0 24 24">
    <path fill="white" d="M12,2A10,10 0 0,1 22,12A10,10 0 0,1 12,22A10,10 0 0,1 2,12A10,10 0 0,1 12,2M7,10L12,15L17,10H7Z" />
</svg>

</a>
</v-row >

<v-row style="color:white" align="center"  justify="center" class="mt-10" > 
 <h3 >
המחזור הקרוב ב <span style="background:orange" >3 אוקטובר תפוסה מלאה </span> 
 </h3>
</v-row>

<v-row align="center" justify="center" class="mt-5 d-flex flex-column" >

  <h3 style="color:white" class="text-center" >
 :המחזורים הבאים  
<h3 style="background:orange" >2021 31 אוקטובר</h3> 
 <h3 style="background:orange" >2021 28 אוקטובר </h3> 
 </h3>

 <h3 style="color:white">קבל עכשיו חוברת במייל מדריך</h3>
  <h3 style="color:white">שתעשה לך הכרות עם עולם והתוכנה ואיך תוכל להפוך למתכנת מהר</h3>
                
</v-row>

<v-row class="pt-5" justify="center">
<v-form class="d-flex" justify="center">
<v-btn
        color="primary"
        elevation="7"
        outlined
        raised
        large
        class="mr-3"
       
          >
         ! תן לי גישה למדריך עכשיו 
          </v-btn>
<v-text-field
            label="מייל"
           placeholder="Placeholder"
            solo
        
          ></v-text-field>  

  </v-form>
</v-row>
  
  
        
         



</v-container>

</template>

<script>
  export default {
    name: 'homePage',

    data: () => ({
      ecosystem: [
        {
          text: 'vuetify-loader',
          href: 'https://github.com/vuetifyjs/vuetify-loader',
        },
      ],
      importantLinks: [
        {
          text: 'Documentation',
          href: 'https://vuetifyjs.com',
        },
       
      ],
      whatsNext: [
        {
          text: 'Explore components',
          href: 'https://vuetifyjs.com/components/api-explorer',
        },
       
      ],
    styleObject: {
     minHeight:'94vh',
     backgroundImage:"linear-gradient(rgba(0,0,0,.8),rgba(0,0,0,.8)), url('https://flashdev.io/img/fdback.bb8842c3.jpg')",
     backgroundSize:'cover',
     backgroundPosition:'center',
     backgroundRepeat:'no-repeat',
     maxWidth:'100%',
     padding:0,
     margin:0,
      }

    }),
  }
</script>



