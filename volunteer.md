---
title: Volunteer
layout: volunteer
---


<style>

.page-wrapper {
  font-family: 'Lato', sans-serif;
  min-height: 100vh;
  margin: auto;
  display: flex;
  z-index:1;
  flex-wrap: wrap;
  align-content: flex-start;
  justify-content: space-evenly;
  padding-left: calc(5% - 16px);
  padding-right: calc(5% - 16px);
  /* padding: 0 5%; */
}


.profile-box {
  border-radius: 3px;
  margin: 12px 12px;
  padding: 12px 12px;
  width: 200px;
  text-align: center;
  transition: 300ms;
  flex-grow: 1;
}


img {
  width: 150px;
  height: 150px;
  border:2px solid #fff;
  border-radius: 50%;
  box-shadow: 0 2px 6px 0 rgba(47,83,151,0.10);
}


</style>


 
 <div class="page-wrapper">
 {% for persons in site.data.volunteer %}
     <div class="profile-box">
     <a href="{{persons.twitter}}" target="_blank"><img src="{{persons.image}}" alt="{{person.name}}"></a>
    <h3 class="subtitle has-text-centered">{{persons.name}}</h3>
    <!--   <h4>[{{persons.role}}]</h4> -->
     </div>
 {% endfor %}
 </div>

