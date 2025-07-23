---
layout: default
hpl_link: "https://www.google.com/maps/place/Hamilton+Public+Library+-+Central+Library/@43.2591682,-79.8729722,17z/data=!3m1!4b1!4m6!3m5!1s0x882c9b83cff8c4a7:0x3afc884c7eec4970!8m2!3d43.2591643!4d-79.8703973!16s%2Fg%2F1tfq58_k?entry=tts&g_ep=EgoyMDI1MDYyMy4yIPu8ASoASAFQAw%3D%3D&skid=a4f273f2-6651-48ab-967d-a5834a1af46e"
mcmaster_link: "https://www.google.com/maps/place/McMaster+Continuing+Education/@43.2572786,-79.8716939,17z/data=!3m2!4b1!5s0x882c9b83994cd1ad:0x7172a94b7544117!4m6!3m5!1s0x882c9b4347d2cf61:0x8ee2e2718bb4c832!8m2!3d43.2572747!4d-79.869119!16s%2Fg%2F11vx6zcfmb?entry=tts&g_ep=EgoyMDI1MDYyMy4yIPu8ASoASAFQAw%3D%3D&skid=c3d2a597-7aca-41af-9c8c-434c6769bcca"
---

<div class="content-container">
    <div class="home-header">
        <div class="image-box" style="position: relative;">
            <img src="{{ site.baseurl }}/assets/images/S&P.png" alt="Central Library"> 
        </div>
    </div>

<h1 class="post-title">Space and Place Conference</h1>

<p>
    McMaster University Libraries, in partnership with Hamilton Public Library and McMaster University's Office of Community Engagement, are excited to announce the inaugural Space and Place conference, taking place on <strong>Friday, October 17, 2025</strong>, at
    <a href="{{ page.hpl_link }}">Hamilton Public Library's Central Branch</a> and
    <a href="{{ page.mcmaster_link }}">McMaster University's Continuing Education centre</a>.
</p>

<p>
    This gathering will celebrate and embrace the different ways Hamilton's communities think about their built and natural environment. We hope to explore perspectives that highlight the ways we think about space and place, including mapping, art, storytelling, and local Indigenous knowledge.
</p>

<p>
    This event is dedicated to fellowship amongst scholars, practitioners, artists, and professionals who explore the spatial dimensions of the Hamilton region in creative and meaningful ways.
</p>

<div class="submissions-box">
    <strong>Now accepting submissions for participation!</strong>
    Visit the <a href="{{ site.baseurl }}/call-for-proposals/">Call for Proposals</a> page for more details and submission form.
</div>

<div id="popup" class="popup-overlay show">
    <div class="popup-box">
        <!-- <button class="close-btn" onclick="closePopup()">×</button>  no need for button--> 
        <div class="submissions-box2">
            <strong>Now accepting submissions for participation!</strong>
            Visit the <a href="{{ site.baseurl }}/call-for-proposals/">Call for Proposals</a> page for more details and submission form.
        </div>
    </div>
</div>

<script>
  function closePopup() { //function to close removes show css which contains opactiy =1
    const popup = document.getElementById("popup");
    popup.classList.remove("show");
    setTimeout(() => {
      popup.style.display = "none";
    }, 500);
  }

  window.onload = function () { //should load at start
    const popup = document.getElementById("welcome-popup");
    if (popup && !sessionStorage.getItem("welcomeShown")) {
      popup.classList.add("show");
      sessionStorage.setItem("welcomeShown", "true");
    }

    const popupOverlay = document.getElementById("popup");
    if (popupOverlay) {
      popupOverlay.addEventListener("click", function (e) { 
        const popupBox = popupOverlay.querySelector(".popup-box"); //whole white box
        if (!popupBox.contains(e.target)) { //check if click is in boxes resgion
          closePopup();
        }
      });
    }
  };
</script>
</div>
