<template>
    <div>
        <div class="columns">
            <div class="column">
                <div class="card">
                    <div class="card-content">
                        <p class="title is-6">Resume and Recommendations
                        </p>
                    </div>
                    <div class="card-content">
                        <p>
                            <a href="https://docs.google.com/document/d/181xOFDRX5Db15ah7LorR8M1lWT3ql4mBmpFdo89sgDE/edit?usp=sharing" target="_blank">Resume</a>
                        </p>
                        <ul>
                            <li>
                                <a href="https://codepen.io/jameshood118/" target="_blank">CodePen</a>
                            </li>
                            <li>
                                <a href="https://github.com/jameshood118/" target="_blank">Github</a>
                            </li>
                            <li>
                                <a href="https://www.linkedin.com/in/jameshood118/" target="_blank">Linkedin</a>
                            </li>
                        </ul>
                        <p>I have had the pleasure of working with some very talented individuals, and I have made an impression:</p>
                    </div>
                </div>
            </div>
        </div>
        <div class="columns is-multiline is-mobile">
            <div class="column is-6" v-for="recs in recommend" :key="recs.person">
                <div class="card">
                    <div class="card-content">
                        <p class="title is-6">{{recs.person}}
                        </p>
                        <p class="subtitle is-7">{{recs.title}}</p>
                    </div>
                    <div class="card-content" v-html="recs.text"></div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
name: "Resumes",
data(){
    return{
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
    }
}
}
</script>

<style>
</style>
