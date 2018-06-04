<template>
  <div>
    <div class="columns">
      <div class="column">
        <div class="card">
          <header class="card-header">
            <p class="card-header-title">
              About</p>
          </header>
          <div class="card-content">
            <p>My name is James Hood, I am a Front end Web Developer. I work with a wide array of tools. My languages include: VueJS, Javascript (ECMAScript 5/6), Jquery, HTML(5), CSS(3). I have worked as a graphic designer and as a web developer, and in my own personal freelance work I have often been both at the same time. In 2015 I acquired new skills in my briefcase, these include: Shipping and Logistics, Ecommerce data entry, Amazon Vendor Central compliance, EDI data exchange as well as Quickbooks online. I have become more than just a Web Developer, and much more than just a face in the crowd.</p>
            <p>These days its refreshing to find someone who can do multiple things, who can learn multiple skills, and run with that. The days of 1 skill per 1 employee are over. That just doesnt work these days.</p>
            <p>I have had the pleasure of working with some very talented individuals, and I have made an impression:</p>
          </div>
        </div>
      </div>
    </div>
    <div class="columns is-multiline is-mobile">
      <div class="column is-6" v-for="recs in recommend" :key="recs.person">
        <div class="card">
          <div class="media-content">
            <p class="title is-5">{{recs.person}}</p>
            <p class="subtitle is-7">{{recs.title}}</p>
            <hr/>
          </div>
          <div class="card-content" v-html="recs.text"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
  data(){
    return {
      recommend: [
      {text:"<p>James has worked as a contractor for our advisor website offering. He learned a new platform for both him and us (Sitecore) and helped migrate >3000 advisor websites from a legacy platform onto the new platform within a very aggressive 6 month time period. He always took on the more complicated sites for the team. Shortly after the initial migration project, we asked James to work on moving more advanced and complex advisor sites onto the new Sitecore platform.</p><p>Moreover, James trained and provided leadership to the other contractors brought on to assist with the migration project. He was helpful and always helped out with side projects as needed. His varied technical skillset from prior roles have been extremely beneficial to our team and we will miss him when his contract ends.</p>", person: "Jennifer Carpenter", title:"Manager, Advisor Marketing Products, Raymond James Financial, Inc."}
      ,{text:"<p>Great attitude and always ready to help. Very knowledgeable and quick in responding to any issues.</p>", person: "Tsvetelina Georgiev", title:"Senior Advisor, Compliance - Corporate Marketing, Raymond James Financial, Inc."}
      ,{text:"<p>James has been an exceptional asset to the team and crucial to various projects we’ve undertaken in our department. He has the technical knowledge to be a resource to other team members and has even leveraged his experience with our platforms to take on leadership tasks. It has been a pleasure working with James.</p>", person: "Olivier Bizimungu", title:"Senior Product Analyst, Raymond James Financial, Inc."}
      ,{text:"<p>James is very quick to respond to questions and concerns. His knowledge and expertise can always be counted on. He has truly been an asset and ‘go to’ for my team and I. He is also always very friendly and understanding of the business needs.</p>", person: "Michelle Wooten", title:"Manager, Compliance Advertising, Raymond James Financial, Inc."}
      ,{text:"<p>James is a hard worker and extremely helpful. He knows his stuff and is happy to assist in anyway. He would be a great asset to any firm.</p>", person: "Jessica Custer ", title:"Marketing Coordinator, Raymond James Financial, Inc."}
      ,{text:"<p>James is a great cross-functional partner to have on any team. He has always done a great job in communication as well as execution for site updates. I value the fact that he lets me know if a problem may potentially arise well in advance. If there ever is a problem he always stayed in constant communication with his cross-functional partners till the resolution is executed.</p><p>During the time I worked with James, I truly valued his hard work and dedication.</p>", person:"Morgan Bright-Ferrone ", title:"Assistant Manager, Digital Commerce Marketing Chico's)"}
      ,{text:"<p>James Hood has worked with me since December last year. He has been challenged with new approaches at Chico's FAS, and new platforms we have been testing. He manages to get a hang of a system relatively fast, and is a hard worker and definitely devoted to getting the job done.</p>", person: "Claudia Klees", title:"Creative Developer, Contract"}
      ,{text:"<p>I've never met a more devoted, flexible and versatile employee than James. He's dedicated to the success of Marbles' Boxa brand across multiple web platforms. He understands the intricate workings of our e-commerce platforms and isn't afraid to raise new ideas or try new campaigns in an effort to generate sales.</p><p>James is a team player and an asset to Marbles. The company is lucky to have him.</p>", person: "Elizabeth Carlton", title:"Author, Copywriter, Editor, Marbles, LLC"}
      ,{text:"<p>I’ve had the pleasure of working with James. He always finished his work in time and took initiative to go beyond what was asked. His expertise in e-commerce helped Marbles and its sales significantly. His skills in web development facilitated in web design. Working with him was a pleasure and he will be a great asset to any company.</p>", person: "Gihoon Song", title: "Industrial Designer, Marbles, LLC"}
      ,{text:"<p>James is a full stack web developer with a “can-do” attitude. He has an extremely versatile skill set and an amazing ability to multi-task. James can be inserted into any difficult project or task and he will quickly assess the project’s need and then develop an action plan. Finally and most importantly, James remains calm in high-stress situations and finishes projects on time.</p>", person: "Tony Monda", title:"Vice President of Strategic Marketing"}
      ],
      generalList: [
        {item: "Tabletop RPG's"},
        {item: "MMORPG's (World of Warcraft, Star Wars: The Old Republic, WildStar)"},
        {item: "reading various books (sometimes coding, sometimes scifi/fantasy)"},
        {item: "reading random wikipedia entries"},
        {item: "Listening to music (all sorts)"},
        {item: "Playing Guitar (real guitar, not guitar hero, cant play that to save my life)"},
        {item: "Video Games (Star Wars Force Unleashed, Portal)"},
        {item: "Watching movies with my fiance!"},
        {item: "Playing card games with friends (Cards Against Humanity, Munchkin)"},
        {item: "Nerf Guns - Learning how to mod, and trying to organize a Humans Vs Zombie League"} ],
      gamesList: [
        {item: "World of Warcraft"}, 
        {item: "Diablo 3"}, 
        {item: "WildStar"}, 
        {item: "Star Wars: The Old Republic"}, 
        {item: "Infamous: Second Son"}, 
        {item: "101 Ways to Die (PS4)"}], 
      tvList: [
        {item: "Archer"},
        {item: "The IT Crowd"},
        {item: "Big Bang Theory"},
        {item: "Heroes"},
        {item: "Community"},
        {item: "Good Eats"},
        {item: "Modern Marvels"},
        {item: "How its Made"},
        {item: "How I Met Your Mother"},
        {item: "Game of Thrones"},
        {item: "Lost"},
        {item: "The Walking Dead"},
        {item: "Once Upon a Time"},
        {item: "Iron Chef (both Original and American)"},
        {item: "House, MD"},
        {item: "Orange is the New Black"},
        {item: "Scrubs"}],
      heroList: [
        {item: "Deadpool"}, 
        {item: "Wolverine"}, 
        {item: "Nightcrawler"}, 
        {item: "Batman"}, 
        {item: "Gambit"} ],
    }
  }

}
</script>

<style scoped>
.title {
  padding-top: 5px;
}
.title,
.subtitle {
  padding-left: 5px;
}
</style>
